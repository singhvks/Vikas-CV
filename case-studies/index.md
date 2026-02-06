# Productionized Case Studies

This page presents selected case studies covering production-grade ML and LLM systems designed and implemented under real enterprise constraints. Each case study focuses on architectural decisions, data and model trade-offs, and operational considerations such as cost control, governance, scalability, and reliability.

---

### Case Study 1: LLM-Augmented Weekly Business Review (WBR) System

**Objective**  
Design and deploy a scalable, cost-controlled LLM-augmented analytics system to automate weekly and monthly executive business reviews, replacing manual, error-prone analysis workflows used by category managers and senior leadership.

The system standardizes narrative insights across multiple business dimensions while operating on **TB-scale transactional data**, with strict requirements around **interpretability, reproducibility, and budget governance**.

**What this case study covers**
- Designing an **OLAP-first analytics pipeline** for high-volume, multi-dimensional reporting
- Feature engineering under **enterprise reporting and data-consistency constraints**
- **LLM selection, prompt design, and cost/latency trade-offs** at scale
- **FastAPI-based service separation** between analytics, application logic, and AI inference
- **Governance mechanisms** including caching, rate limiting, and budget controls for sustained LLM usage

**Design Philosophy**  
This system was intentionally built as a **batch-oriented, enterprise-grade analytics platform**, prioritizing consistency, explainability, and operational reliability over real-time inference. The LLM augments human decision-making rather than replacing core BI or financial controls.

➡️ **[Read full case study →](./category-analytics-agentic/)**

### Case Study 2: Geospatial ML–Driven New Store Site Selection & Sales Forecasting

**Objective**  
Design and deploy a production-grade geospatial machine learning system to support **New-to-Industry (NTI) retail site selection** for a **$10B+ convenience and prepared foods retailer (2,500+ locations)**.  
The goal was to replace decentralized, intuition-driven real estate decisions with a **standardized, explainable, and scalable forecasting engine** capable of estimating **3-year category-wise sales** from a simple latitude/longitude input.

The system directly informs **multi-million dollar CAPEX decisions**, where errors translate into long-term lease risk and irreversible investment commitments.

**What this case study covers**
- Large-scale **geospatial feature engineering** across census, mobility, traffic, and infrastructure datasets using **Spark on Databricks**
- Designing a **dual trade-area framework** (drive-time isochrones and radial distances) to model real-world accessibility and customer behavior
- **Cold-start modeling strategies** for NTI locations using clustering-based “statistical twins”
- Multi-vertical **XGBoost forecasting architecture** (fuel, diesel, prepared food, grocery)
- **Explainability-first ML design** using SHAP to support executive trust and auditability
- Production deployment using **MLflow, Delta Lake, and serverless model serving**, with cost and drift governance

**Design Philosophy**  
This system was intentionally built as a **spatial-first, cross-sectional modeling platform**, prioritizing *where* a store is over *when* it opens. Architectural choices favored **interpretability, reproducibility, and operational scalability** over purely academic modeling approaches, ensuring the solution could be trusted and adopted by real estate and finance leadership at enterprise scale.

➡️ **[Read full case study →](./site-selection-nti/)**

---

*(More case studies will be added here, covering ML platforms, LLM pipelines, and large-scale data engineering systems.)*
