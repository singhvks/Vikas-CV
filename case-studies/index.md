# Case Studies

Production-grade AI and ML systems designed and implemented under real enterprise constraints - scale, cost, governance, and client accountability. Each case study documents architectural decisions, data and model trade-offs, and operational considerations including cost control, explainability, and regulatory compliance.

---

## Case Study 1: Multi-Agent GenAI Analytics Platform

**Client Engagement:** Large-scale eCommerce client  
**Role:** Principal Architect  
**Impact:** $100K/yr saved · 40 FTE automated · 65% inference cost reduction · 1,000+ concurrent users

**Objective**  
Design and deploy a scalable, cost-controlled multi-agent GenAI platform to automate weekly and monthly executive business reviews for category managers and senior leadership, replacing manual, error-prone analysis workflows operating on TB-scale transactional data.

**What this case study covers**
- Designing an **OLAP-first analytics pipeline** for high-volume, multi-dimensional reporting
- **Custom async routing architecture**: evaluated LangGraph, selected a purpose-built FastAPI async router for lower latency at production scale
- **LLM-as-Judge evaluation framework** and human-in-the-loop output quality pipeline
- **Cost-governance architecture**: semantic caching, token budgeting, dynamic model routing - achieving 65% inference cost reduction ($8 → $2.50/request)
- **FastAPI service separation** between analytics, application logic, and AI inference
- Scaled to support **10,000 concurrent users** with sub-100ms latency targets

**Design Philosophy**  
Built as a **batch-oriented, enterprise-grade analytics platform** prioritising consistency, explainability, and operational reliability over real-time inference. The LLM augments human decision-making rather than replacing core business controls.

➡️ **[Read full case study →]({{ '/case-studies/category-analytics-agentic/' | relative_url }})**


---

## Case Study 2: Geospatial ML - New Store Site Selection &amp; Sales Forecasting

**Client Engagement:** $10B+ convenience &amp; prepared foods retailer (2,500+ locations)  
**Role:** Lead Architect  
**Impact:** $50M+/month CAPEX informed · 70% faster approval cycles (3 weeks → 5 days) · 22× query latency improvement · 15% accuracy lift vs 3rd-party tool

**Objective**  
Design and deploy a production-grade geospatial ML system to support new-store site selection, replacing decentralised, intuition-driven real estate decisions with a **standardised, explainable, and scalable forecasting engine** capable of estimating 3-year category-wise sales from a latitude/longitude input.

The system directly informs **$50M+ monthly CAPEX allocation decisions**, where errors translate into long-term lease risk and irreversible investment commitments.

**What this case study covers**
- Large-scale **geospatial feature engineering** (200M+ features) across census, mobility, traffic, and infrastructure datasets using Spark on Databricks
- **Dual trade-area framework** (drive-time isochrones + radial distances) for real-world accessibility modelling
- **Cold-start modelling** via clustering-based statistical twins for new-to-industry sites
- Multi-vertical XGBoost forecasting (fuel, diesel, prepared food, grocery) with SHAP explainability
- Migration from schema-on-read Hive to **star-schema Delta + Unity Catalog**: query latency from 45s → &lt;2s (22× improvement)
- Production deployment using **MLflow, Delta Lake, and serverless model serving**

**Design Philosophy**  
Built as a **spatial-first, cross-sectional modelling platform** prioritising interpretability, reproducibility, and operational scalability. Architectural choices ensured the solution could be trusted and adopted by real estate and finance leadership at enterprise scale.

➡️ **[Read full case study →]({{ '/case-studies/site-selection-nti/' | relative_url }})**


---

## Case Study 3: Bayesian MCMC Clinical Trial Enrollment Forecasting - Oncology Supply Chain

**Client Engagement:** Global Pharmaceutical Client (Top-10 Oncology Biopharma) - Phase 2/3 clinical trials  
**Role:** ML Engineer & Data Engineering Lead · MLOps Architect  
**Impact:** ~$2B projected supply waste avoidable · 2× heuristic replaced by 63% MAE forecast (first-ever quantitative model) · 8 trials · 40 countries · 3-year supply plan horizon

**Objective**  
Design and deploy a **site-level probabilistic enrollment forecasting system** for oncology trials, replacing a blanket 2× over-ordering safety stock heuristic with a Bayesian MCMC model that generates 80% confidence enrollment projections per site, per country, for a 3-year forward horizon - feeding directly into SAP IBP for drug and placebo supply planning.


The problem required solving for **patient attrition, site-level data sparsity, blinded trial supply complexity, and cross-site patient transfers tracked via IRT**, at a scale of 40 countries and 80+ trial sites simultaneously.

**What this case study covers**
- **Gamma-Poisson Bayesian inference**: site-level enrollment modelled as a Poisson process with Gamma-distributed rate - enabling native probabilistic uncertainty quantification from sparse monthly data (1–5 patients/site/month)
- **Hierarchical MCMC prior elicitation**: country × TA × phase × indication distribution fitting with fallback cascade for cold-start sites (PyMC3 NUTS sampler, 2000 samples, 90% burn-in)
- **Bayesian conjugate reforecasting**: mid-trial posterior updates using IRT actuals (Gamma(α+k, β+v)) - no model retraining required
- **IRT-based patient transfer reconciliation**: engineering layer to distinguish true attrition from inter-site patient transfers using patient tracking IDs and dropout reason codes
- **AWS data platform**: Glue ETL pipelines, 3-zone S3 data lake, MICE imputation, CloudWatch monitoring
- **Enterprise integration**: flat-file monthly batch delivery to SAP IBP for supply planning; Veeva Vault writeback; MLflow model governance

**Design Philosophy**  
Built as a **Bayesian-first, hierarchical probabilistic system** where uncertainty is a first-class output. The 80% credible interval - not a point forecast - is the primary deliverable, enabling supply planners to make defensible safety stock decisions without systematic over-ordering.

➡️ **[Read full case study →]({{ '/case-studies/mcmc-clinical-trial-enrollment/' | relative_url }})**


---

*(Additional case studies covering enterprise demand forecasting, MLOps platforms, and LLM pipeline architecture will be added.)*
