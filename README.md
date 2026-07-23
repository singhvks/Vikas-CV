# Vikas Kumar Singh

**Manager, Agentic AI @ eBay &nbsp;|&nbsp; AI/Backend Architect specializing in Agentic Systems**

Bangalore, India

<sub>
📧 <a href="mailto:singhvks@outlook.in">Email</a> · <a href="https://linkedin.com/in/singhvks">LinkedIn</a> · <a href="https://singhvks.github.io/Vikas-CV">Portfolio</a> · 💻 <a href="https://github.com/singhvks">GitHub</a> · 📄 <a href="https://docs.google.com/document/d/11G7DIVcDr3NbY4Yd-_yJ6ADBa5IMo7mRaW0_0VfW8dc/preview">View CV</a> · ⬇️ <a href="https://docs.google.com/document/d/11G7DIVcDr3NbY4Yd-_yJ6ADBa5IMo7mRaW0_0VfW8dc/export?format=pdf">Download PDF</a>
</sub>

---

## Business Impact

| Metric                                        | Value                        |
| --------------------------------------------- | ---------------------------- |
| Supply chain waste prevented                  | **$2B** over 5 years         |
| Monthly CAPEX allocation decisions informed   | **$50M+**                    |
| Annual system maintenance overhead eliminated | **$1M+**                     |
| BI vendor licensing eliminated                | **$2M+**                     |
| Manual reporting FTEs automated               | **40 FTE**                   |
| LLM inference cost reduction                  | **65%** ($8 → $2.50/request) |
| Query latency improvement                     | **22×** (45s → <2s)          |
| Site-selection approval cycle reduction       | **70%** (3 weeks → 5 days)   |
| GenAI platform scaling target                 | **5,000 users** *(in progress)* |
| Operations platform savings target            | **4,000+ man-hours/year** *(in progress)* |

---

## Profile

**AI Systems Architect &amp; Principal Engineer** with 10 years of experience designing and implementing production-grade AI platforms, multi-agent systems, and enterprise data infrastructure across regulated sectors (pharma, retail, healthcare, and financial services). Drives technical execution on high-stakes systems, transforming complex data challenges into scalable, high-performance architectures.

Built and shipped end-to-end production systems in a **forward-deployed capacity** — serving as the hands-on design authority for low-latency, high-concurrency solutions. Now directing **technical architecture and system strategy for Agentic AI at eBay India**, continuing that end-to-end engineering ownership model from inside the organisation.

Led technical delivery and mentored engineering teams of **4–28 developers** across Fortune 500 engagements. Combines deep technical execution (FastAPI, Databricks, PySpark, custom ML/LLM routing) with architectural leadership, personally authoring core components and defining key systems patterns.

---

## Core Expertise

### GenAI &amp; LLM Systems

- Multi-Agent Orchestration (LangChain, LangGraph, MCP)
- RAG Architecture &amp; Retrieval Optimisation
- LLM-as-Judge Evaluation Frameworks &amp; Human-in-the-Loop Review
- Token Budgeting, Semantic Caching &amp; Dynamic Model Routing
- Prompt Engineering, Output Validation &amp; Cost Governance

### System Design &amp; Backend Engineering

- API Design Patterns &amp; Service Architecture
- Service Decomposition &amp; Scalability Trade-offs
- Caching &amp; Queueing Strategy
- OIDC / OAuth2 Authentication Design
- Async FastAPI (concurrent request handling, batching, connection pooling)

### Data &amp; Platform Architecture

- Databricks Lakehouse (Medallion Architecture, Unity Catalog, Delta Lake)
- PySpark - billion-row pipelines, dynamic partitioning
- AWS Glue & S3, DuckDB, OLAP design
- Geospatial Feature Management (200M+ features)

### ML, MLOps &amp; Engineering

- Bayesian MCMC, XGBoost, SHAP Explainability
- MLflow — model versioning, A/B testing, drift detection, audit logging
- Docker, Kubernetes, CI/CD
- Regulated Systems: HIPAA / GDPR / Solvency II compliance architecture

---

## Selected Case Studies

**Production systems designed under real-world scale, governance, and cost constraints.**  
👉 [Read all case studies](./case-studies/)

---

### Principal Architect - Multi-Agent GenAI Analytics Platform (eCommerce)

**Client:** Large-scale eCommerce client &nbsp;·&nbsp; **Impact:** $100K/yr saved · 40 FTE automated · 65% inference cost reduction

Designed and delivered a production-grade GenAI platform for executive analytics and compliance reporting, replacing fragmented manual workflows across category managers and senior leadership.

- Async FastAPI–based **multi-agent service architecture**, decoupled AI service from application logic
- Replaced 40 FTE of manual analysis with agentic orchestration - **60 reports/week** automated
- **Cost-governance layer**: token budgeting, semantic caching, dynamic LLM routing - cut inference cost from **$8 → $2.50/request** (65% reduction)
- **Custom async routing layer** (benchmarked against LangGraph; custom implementation selected for lower latency at scale)
- **LLM-as-Judge evaluation framework** with human-in-the-loop review pipeline for output quality assurance
- Scaled to **10,000 concurrent users**; designed for sub-100ms latency at 1,000+ concurrent users
- Enterprise SSO–based access control, prompt sanitisation, and audit trails

**Outcome:** $100K/year operational overhead eliminated · 1,000+ concurrent users · &lt;100ms latency

➡️ **[Read full case study →](./case-studies/category-analytics-agentic/)**

---

### Lead Architect - Geospatial ML Site Selection &amp; Sales Forecasting (Retail)

**Client:** $10B+ convenience &amp; prepared foods retailer (2,500+ locations) &nbsp;·&nbsp; **Impact:** $50M+/month CAPEX informed · 70% faster approvals

Architected a **Databricks Lakehouse–based geospatial ML platform** to support new-store site selection, replacing intuition-driven real estate decisions with a standardised, explainable forecasting engine.

- Migrated from schema-on-read Hive to **star-schema Delta + Unity Catalog**; designed dynamic partitioning for **200M geospatial features**
- Query latency: **45s → &lt;2s (22× improvement)**
- Medallion architecture processing **&gt;1TB** of transactional, mobility, US census, and infrastructure data
- Dual trade-area framework (drive-time isochrones + radial rings) for real-world accessibility modelling
- Cold-start forecasting via clustering-based **statistical twin** methodology
- Multi-vertical XGBoost regressors (fuel, diesel, prepared food, grocery) with SHAP explainability
- **MLflow and Unity Catalog** governance, lineage, and model lifecycle management
- **15% accuracy lift** over industry-standard 3rd-party benchmarking tool

**Outcome:** $50M+/month CAPEX allocation decisions informed · 3 weeks → 5 days approval cycle (70% reduction)

➡️ **[Read full case study →](./case-studies/site-selection-nti/)**

---

## Professional Experience

### eBay India — Manager, Agentic AI

*Bangalore, India · Jul 2026 – Present*

- Scaling the production GenAI platform to **5,000 users** and architecting an operations platform targeted to save **4,000+ man-hours annually** *(in progress)*.
- Designed and built backend service architecture (async FastAPI, service decomposition, caching layer) supporting the GenAI analytics platform at **1,000+ concurrent enterprise users at &lt;100ms latency**, automating 60 reports/week and eliminating **$100K/year** operational overhead.
- Implemented SSO authentication (OIDC) for role-based access control across enterprise user tiers.
- Implemented LLM cost-governance layer (token budgeting, semantic caching, dynamic model routing) — cutting inference costs **65%** while maintaining output quality.

---

### Tredence Analytics — Data Science Manager &amp; Principal AI Architect

*Bangalore, India · Nov 2024 – Jul 2026 · **Deployed to large-scale eCommerce client as embedded AI Architect, Aug 2025 – Jul 2026***

- Directed and executed a **1TB+ Geospatial Lakehouse migration** for Retail Real Estate site-selection — applying ISRO-certified geodata analysis techniques — improving query latency **22× (45s → &lt;2s)** and accelerating site-selection approval from **3 weeks to 5 days**, informing **$50M+ monthly CAPEX decisions**.
- Designed Databricks-based data engineering pipelines and GenAI model hosting (RAG-based) for **product harmonization across a US retail footwear brand's outlets in 50+ countries** — enabling automated cross-region rerouting to resolve out-of-stock issues.
- Decommissioned legacy on-prem ETL and migrated to AWS Glue + Databricks — achieving **30% cloud cost reduction** and eliminating **$1M+/year** system maintenance overhead.
- Enabled the **AI Centre of Excellence (CoE)** through multiple solution and architecture designs for retail clients — reducing client implementation and planning timelines by **50%**.

---

### ZS Associates - Business Technology Solutions Consultant, AI Systems

*Pune, India · Apr 2021 – May 2024*

- Architected demand forecasting engine for a **$10B+ pharmaceutical client**: Bayesian MCMC over standard econometrics (native uncertainty quantification, faster convergence on irregular clinical patterns). Spark feature pipeline (**500M+ SKU-day pairs**), end-to-end ownership from model R&D to MLOps. Economic outcome: **$2B supply chain waste prevention over 5 years**.
- Implemented Spark-based next-best-action recommendation engine for MSL/KOL engagement, interfacing Veeva CRM with MLflow model monitoring and feature drift response.
- Scaled AI delivery organisation: MLOps platform enabling **28 distributed engineers to ship 6 concurrent enterprise projects** without bottlenecks. Built compliance automation layer ensuring HIPAA/GDPR validation on every model commit.

---

### Collabera Technologies - Data Engineer

*Pune, India · Sep 2020 – Apr 2021*

- Architected HIPAA-compliant Real-World Data (RWD) platform: PII detection, field-level encryption, audit logging. Processed **500M+ healthcare records/day** with &lt;10MB per-patient data footprint. Integrated Komodo data for HCP scoring.
- Eliminated BI vendor dependency (**$2M+ contract cycle**): custom Python analytics layer with sub-second response on 100M+ patient records.

---

### L&amp;T Infotech - Engineer

*Pune, India · Sep 2016 – May 2020*

- Owned ML-driven insurance risk platform: API-integrated model serving at **sub-50ms inference SLA**, multi-armed bandit A/B testing for 10+ concurrent models, feature store for **500+ features with drift detection**.
- Engineered GDPR/Solvency II compliant Spark ETL: immutable transaction logs, cryptographic data lineage, automated compliance validation on every pipeline run.

---

## Certifications

- **Generative AI Solutions Architect (2025)**
- **Databricks Certified GenAI Engineer (2025)**
- AI/ML for Geodata Analysis - ISRO
- Master of Science, Applied Data Science - WorldQuant University (2021)
- Certified NLP Developer - Vskills
- Certified Python Developer - Vskills
- Certified Tableau Author - Tableau
- Math for Machine Learning - Amazon

---

## Education

- **B.Tech, Electronics Engineering** - BVDU College of Engineering, Pune (2016)
- **Master of Science, Applied Data Science** - WorldQuant University (2021)
- Diploma, Network Security - BVDU College of Engineering, Pune (2015)

---

## Languages

- English - Full Professional Proficiency (C2)

