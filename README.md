# Awesome-Supplier-Relationship-Management-SRM

## Top Supplier Relationship Management (SRM) Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Supplier Onboarding, Performance Management & Supply Base Governance*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Supplier Relationship Management (SRM)**. These tools enable organizations to manage the complete supplier lifecycle—from registration and qualification through performance monitoring, risk assessment, and collaborative sourcing—while maintaining compliance and driving supply base value.



**Examples** include Workday Supplier Relationship Management, SAP Ariba, Coupa, Ivalua, Jaggaer, GEP SMART, Tealbook, Graphite Connect, HICX, and Apex Analytix (the category leaders).



**Open-source emphasis**: SRM is a domain where open-source tooling is **emerging but fragmented**. The strongest active project is **mcp-supplier** (zavora-ai), which provides a broad SRM backbone with 34 MCP tools covering qualification, certifications, RFQ, quality audits, scorecards, and risk monitoring. Other projects focus on procurement workflows (VendSync, VendorBridge AI) or supplier onboarding (Supplier Master AI) but lack the full SRM relationship-management depth. Teams seeking complete enterprise SRM should evaluate commercial platforms or plan for significant custom integration.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Workday Supplier Relationship Management](https://www.workday.com/)**  

  SRM capabilities within Workday's spend management suite, integrating supplier onboarding, qualification, performance tracking, and risk management with procurement and financial workflows.



- **[SAP Ariba](https://www.sap.com/)**  

  Comprehensive supplier management within Ariba's source-to-pay suite; covers supplier qualification, onboarding, performance management, and risk monitoring across the Ariba Network.



- **[Coupa](https://www.coupa.com/)**  

  Supplier information management with onboarding, risk scoring, and performance tracking integrated with Coupa's broader spend management platform.



- **[Ivalua](https://www.ivalua.com/)**  

  Supplier lifecycle management with onboarding portals, diversity tracking, and performance scorecards for enterprise procurement teams.



- **[Jaggaer](https://www.jaggaer.com/)**  

  Supplier management suite with qualification, onboarding, risk assessment, and performance monitoring for direct and indirect procurement.



- **[GEP SMART](https://www.gep.com/)**  

  Unified procurement platform with supplier lifecycle management, onboarding, qualification, and performance tracking integrated with sourcing and contract management.



- **[Tealbook](https://www.tealbook.com/)**  

  Supplier data platform with AI-powered supplier discovery, enrichment, and diversity classification to improve supplier lifecycle visibility and onboarding speed.



- **[Graphite Connect](https://www.graphiteconnect.com/)**  

  Supplier engagement and onboarding platform that centralizes supplier information, compliance documents, and communication for procurement teams.



- **[HICX](https://www.hicx.com/)**  

  Supplier experience management platform focused on supplier master data management, onboarding, and self-service portals to reduce supplier friction.



- **[Apex Analytix](https://www.apexanalytix.com/)**  

  Supplier management and recovery audit platform with supplier onboarding, data validation, and compliance monitoring for AP and procurement teams.



## Open-Source GitHub Projects



- **[mcp-supplier (zavora-ai)](https://github.com/zavora-ai/mcp-supplier)**  

  The most comprehensive open-source SRM platform available (v1.1.0); modeled as a general SRM/procurement backbone (à la SAP Ariba/Coupa/Jaggaer) with **34 MCP tools** covering the full supply base lifecycle: supplier lifecycle status (prospect → active → on-hold/suspended/disqualified), qualification gating PO approval, ISO/IATF/HACCP certification expiry tracking, multi-source catalog pricing with `find_item_sources` ranking, purchase orders with approval gates, RFQ/sourcing with quote comparison and award, quality audits with auto-SCAR on failure, performance scorecards (OTD, quality rate, PPM, composite A–D rating), and supply-risk monitoring with likelihood×impact assessment; includes full audit trail and governance gates on high-impact writes; sample data is fictitious; suitable for electronics, food & beverage, manufacturing, and retail replenishment agent use cases .



- **[VendSync (BidFlow)](https://github.com/RavalMunjal/VendSync)**  

  Full-stack procurement and vendor management ERP (React/Node.js/MongoDB) digitizing the entire purchasing lifecycle from RFQ creation to invoice generation; features role-based access (Admin, Manager, Procurement Officer, Vendor), vendor portal for independent quotation submission, side-by-side quotation comparison with lowest-price highlighting, structured approval workflows with remarks, auto-generated POs and invoices with PDF export, and real-time analytics dashboards . **This is a procurement workflow tool, not a full SRM relationship platform**—it manages transactions and vendor submissions but lacks supplier qualification gating, certification tracking, and performance scorecards.



- **[VendorBridge AI](https://github.com/vatsalgajera-tech/VendorBridge-AI)**  

  AI-powered procurement ERP covering vendor management with risk scoring (based on performance metrics), RFQ creation with multi-vendor assignment, quotation comparison with AI ranking on price/delivery/rating/history, multi-stage approval workflows, purchase order generation from accepted quotes, invoice management, and activity audit logs; React/Node.js/MongoDB stack with role-based access . **Procurement-focused**—provides vendor directory and risk scoring but not the qualification lifecycle, certification management, or quality audit workflows characteristic of SRM platforms.



- **[Supplier Master AI](https://github.com/danillofratta/supplier-master-ai)**  

  Governed enterprise supplier onboarding reference implementation with RAG, Amazon Bedrock, LangGraph, MCP, and human-in-the-loop controls; separates probabilistic AI (policy interpretation, risk recommendation) from deterministic business authority (workflow transitions, SAP integration); includes React operations console, Python/FastAPI services, PostgreSQL, OpenSearch vector retrieval, and transactional outbox/inbox patterns . **Onboarding-focused**—addresses supplier master data creation and governance but not ongoing performance management or sourcing workflows.



- **[Procuman Community Edition](https://github.com/procuman/procuman-community-edition)**  

  Free e-procurement extension for EspoCRM covering supplier management with categorization and relationship tracking, product catalog with supplier associations, and purchase order creation with automated calculations and PDF generation . **Procurement-adjacent**—provides supplier database and PO creation but lacks SRM-specific capabilities like qualification, scorecards, and risk monitoring.



### Additional Strong Open-Source Options



- **GitHub `supplier-management` topic** — Community repositories focus on procurement vendor portals (vendor onboarding, purchase orders, performance tracking) or TPRM/risk assessment tools, not full SRM relationship platforms. Quality and maintenance vary widely.

- **No mature open-source SRM exists** for the complete enterprise workflow of supplier registration → qualification → certification tracking → performance scorecards → risk monitoring → collaborative sourcing. **mcp-supplier** is the closest to a full SRM backbone but is designed as an MCP server for AI agents rather than a standalone web application with UI.



**Frameworks for building custom systems**: **mcp-supplier** provides the most complete open-source SRM foundation with qualification gating, certification tracking, scorecards, and risk monitoring—but requires an MCP client or custom UI for human interaction. **VendSync** or **VendorBridge AI** can serve as procurement workflow layers (RFQ → quote → PO → invoice) but lack SRM relationship depth. **Supplier Master AI** demonstrates governed onboarding patterns with AI governance. A complete SRM system would require integrating these components with custom development for supplier portals, performance dashboards, and certification management workflows.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- SRM platforms handling supplier data and contracts must comply with applicable procurement regulations, anti-corruption laws, and data privacy requirements; supplier qualification and performance data may be subject to audit.

- **Open-source SRM remains fragmented**—mcp-supplier provides a broad SRM backbone but as an MCP server rather than a complete web application; VendSync and VendorBridge AI focus on procurement transactions; Supplier Master AI focuses on onboarding governance. Organizations requiring full SRM with supplier portals, performance dashboards, and certification management should plan for commercial platforms or substantial custom development.

- Verify license terms for commercial use; mcp-supplier is an open-source MCP server , VendSync and VendorBridge AI are independent open-source projects , and Supplier Master AI is a reference implementation .



---



**Made for procurement leaders, supplier managers, supply chain analysts, and vendor relationship owners.**  

Let's make supplier relationship management more open, qualified, and performance-driven.
