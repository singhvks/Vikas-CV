# Productionized Case Studies

This page presents selected case studies covering production-grade ML and LLM systems designed and implemented under real enterprise constraints. Each case study focuses on architectural decisions, data and model trade-offs, and operational considerations such as cost control, governance, scalability, and reliability.

---

## Case Study 1: LLM-Augmented Weekly Business Review System

**Objective:**  
Design and deploy a scalable, cost-efficient LLM-based system to automate weekly and monthly category performance reviews across multiple business dimensions, replacing manual, error-prone analysis workflows used by category managers and senior leadership.

**What this case study covers:**
- Designing an OLAP-first data pipeline over TB-scale transactional data  
- Feature engineering under enterprise reporting constraints  
- LLM selection, prompt design, and cost/latency trade-offs  
- FastAPI-based service separation for application logic and AI inference  
- Governance, caching, and budget controls for large-scale LLM usage  

This system was built to operate reliably in a **batch-oriented, enterprise environment**, prioritizing interpretability, consistency, and operational efficiency over real-time inference.

➡️ **[Read full case study →](./category-analytics-agentic/)**

---

*(More case studies will be added here, covering ML platforms, LLM pipelines, and large-scale data engineering systems.)*
