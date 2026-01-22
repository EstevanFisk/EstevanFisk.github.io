---
title: "R-Powered Strategic Retail Intelligence: From Performance Audit to Market R&D"
summary: "DoD-grade auditability in retail ML: XGBoost pricing & UMAP high-dimensional discovery."
date: 2025-11-10
authors:
    - admin
content_meta:
  content_type: 'Notebook'
links:
  - type: code
    name: GitHub Repo
    url: https://github.com/EstevanFisk/bike_business_analysis_rmarkdown
    icon: brands/github
  - type: code
    name: Interactive Sales Dashboard
    url: "/uploads/notebooks/bike_bus_analysis_rmd/sales_report.html"
  - type: code
    name: Gap Analysis Report
    url: "/uploads/notebooks/bike_bus_analysis_rmd/new_product_recommendation.html"
  - type: code
    name: Customer Segmentation Report
    url: /uploads/notebooks/bike_bus_analysis_rmd/customer_segmentation.html"
tags:
  - R
  - R-Markdown
  - Dashboard
  - Prediction
  - Feature Engineering
  - Customer Segmentation
  - sales
  - pricing
sitemap: true
share: false
#weight: 30
draft: false
---

<div style="display: flex; justify-content: center; flex-wrap: wrap; gap: 4px; margin-bottom: 0px; margin-top: -50px; transform: scale(1.25); transform-origin: center;">
  <a href="https://en.wikipedia.org/wiki/Data_science"><img src="https://img.shields.io/badge/Role-Data_Scientist-0077B5?style=flat&logo=googlesheets&logoColor=white" alt="Role: Data Scientist"></a>
  <a href="https://en.wikipedia.org/wiki/Statistics"><img src="https://img.shields.io/badge/Education-M.S._Statistics-C41E3A?style=flat&logo=icloud&logoColor=white" alt="Education: M.S. Statistics"></a>
  <a href="https://rmarkdown.rstudio.com/"><img src="https://img.shields.io/badge/Methodology-Auditable_Code--Folding-276DC3?style=flat&logo=rstudio&logoColor=white" alt="Methodology: Auditable Code-Folding"></a>
</div>

<div style="display: flex; justify-content: center; flex-wrap: wrap; gap: 4px; margin-bottom: 0px; margin-top: -50px; transform: scale(1.25); transform-origin: center;">
  <a href="https://www.r-project.org/"><img src="https://img.shields.io/badge/Language-R-276DC3?style=flat&logo=r&logoColor=white" alt="R Language"></a>
  <a href="https://rmarkdown.rstudio.com/"><img src="https://img.shields.io/badge/Reporting-R_Markdown-276DC3?style=flat&logo=rstudio&logoColor=white" alt="R Markdown"></a>
  <a href="https://www.tidymodels.org/"><img src="https://img.shields.io/badge/Framework-Tidymodels-orange?style=flat" alt="Tidymodels Framework"></a>
  <a href="https://xgboost.ai/"><img src="https://img.shields.io/badge/Engine-XGBoost-black?style=flat" alt="XGBoost Engine"></a>
</div>

<div style="display: flex; justify-content: center; flex-wrap: wrap; gap: 4px; margin-bottom: -20px; margin-top: -50px; transform: scale(1.25); transform-origin: center;">
  <a href="https://shiny.posit.co/"><img src="https://img.shields.io/badge/App-Shiny_Dashboard-176BEF?style=flat&logo=rstudio&logoColor=white" alt="Shiny Dashboard"></a>
  <a href="https://plotly.com/"><img src="https://img.shields.io/badge/Viz-Interactive_Plotly-4472c4?style=flat&logo=plotly&logoColor=white" alt="Interactive Plotly"></a>
  <a href="https://en.wikipedia.org/wiki/K-means_clustering"><img src="https://img.shields.io/badge/ML-K--Means_Clustering-green?style=flat" alt="K-Means Clustering"></a>
  <a href="https://umap-learn.readthedocs.io/"><img src="https://img.shields.io/badge/Projection-UMAP-yellow?style=flat" alt="UMAP Projection"></a>
</div>

---

Navigating complex data landscapes—across both the **private sector and classified environments within the DoD**—has reinforced the reality that analytical results are only as valuable as the transparency behind them. In high-stakes settings, the "black box" is a liability; every number must be defensible, and every methodology must be auditable.

This suite was born from my experience as a **Product Manager** identifying operational bottlenecks in the sales cycle. By applying a **Master’s-level statistical foundation** to the real-world friction I encountered in the field, I have engineered this project as a gold standard for **Literate Programming**. It transitions from a high-level operational audit to deep-dive market optimization, ensuring that strategic recommendations are always backed by a visible, reproducible technical trail.  

---

### I. Executive Sales Performance Dashboard
### The Operational Source of Truth

This primary module serves as the central hub for the analytical framework, providing a real-time audit of revenue health across geographic markets and product categories.

- **Strategic Focus**: Enables stakeholders to rapidly evaluate revenue concentration and monitor "health and wealth" metrics to optimize resource allocation.

- **Technical Highlight**: Features a reactive backend that facilitates seamless drilling from quarterly trends down to weekly localized performance.

- **The Hub**: Contains direct navigational links to the specialized R&D and Behavioral Intelligence reports below.


<a href="/uploads/notebooks/bike_bus_analysis_rmd/sales_report.html" class="btn btn-primary btn-lg" target="_blank" rel="noopener noreferrer">View Interactive Sales Dashboard</a>

---

### II. Strategic R&D: Algorithmic Gap Analysis
### Portfolio Optimization & Market Benchmarking

Addressing the "Market Entry" problem, this module identifies "blind spots" in the current 97-model fleet to establish high-fidelity pricing benchmarks for new configurations.

- **Strategic Focus**: Discovered two distinct "Blue Ocean" opportunities: an Aluminum-frame Over Mountain line and an Aluminum-frame Triathlon line.

- **Technical Highlight**: Leverages an **XGBoost pricing engine** to establish market benchmarks, ensuring internal price parity before a prototype is built.

- **Validation**: Compares XGBoost against Linear and Random Forest architectures to ensure the most robust predictive accuracy.  


<a href="/uploads/notebooks/bike_bus_analysis_rmd/new_product_recommendation.html" class="btn btn-primary btn-lg" target="_blank" rel="noopener noreferrer">View Gap Analysis Report</a>

---

### III. Behavioral Intelligence: High-Dimensional Market Mapping
### Latent Market Discovery via Clustering

To drive targeted marketing and inventory strategies, this final module uncovers the latent behavioral patterns within a customer base of 30 retail bike shops.

- **Strategic Impact**: Identified four distinct customer profiles, allowing marketing teams to transition from generic outreach to highly targeted, segment-specific campaigns.

- **Technical Methodology**: Employs K-Means clustering and UMAP (Uniform Manifold Approximation and Projection) to project high-dimensional similarity into an intuitive 2D space.

- **The "Practitioner" Difference**: Unlike traditional PCA, the use of UMAP preserves the local structure of the data, providing a more accurate visual representation of distinct customer "landscapes."


<a href="/uploads/notebooks/bike_bus_analysis_rmd/customer_segmentation.html" class="btn btn-primary btn-lg" target="_blank" rel="noopener noreferrer">View Customer Segmentation Audit</a>


---

#### Methodological Note: Built for Auditability
Every report in this suite features **interactive code-folding**. By prioritizing transparency, these documents allow technical peers to inspect the data transformations and model parameters directly inline. This ensures that the methodology is not a "black box," but a fully auditable asset—a requirement I maintain from my background in **regulated and classified environments**.