---
title: 'Experience'
date: 2023-10-24
type: landing

design:
  spacing: '5rem'

# Note: `username` refers to the user's folder name in `content/authors/`

# Page sections
sections:
  - block: resume-experience
    content:
      username: admin
    design:
      # Hugo date format
      date_format: 'January 2006'
      # Education or Experience section first?
      is_education_first: true
  - block: markdown
    content:
      title: 'Data Science Solutions & Business Impact or Predictive Modeling & Advanced Analytics'
      text: |
        - ## End-to-End Model Development
          - Chipotle Mexican Restaurant (CSUF): Developed an **NLP** model in **Python and Streamlit** to analyze and cluster customer comments from both internal and external unstructured text data. This **led to 90% accuracy** in automated comment tagging, enabling efficient insight extraction.
          - Informa: Created a demand elasticity model using **exponential regression** and a propensity-to-buy model using **logistic regression** in R and R-Shiny. Propensity model achieved 85% accuracy, providing valuable insights for sales and marketing strategies.
          - DCMA: Designed and evaluated new forecasting metric for the Department of Defense (DOD) using Brier scoring. Performed **simulations in R and created dashboards in R-Shiny and Power BI**, a project with the potential to save substantial dollars across $5.8 trillion in agency contracts.
          - Wells Fargo: Conducted a **time series analysis in Python** to forecast future workflow growth. The resulting projections for hiring temporary staff during peak periods led to savings of over 250 overtime hours per month.
          - AFCAA: Performed a regression-based cross-check analysis to follow-on acquisition program costs in Python using Dataiku, leading to a 15% correction of estimated ground costs.

        - ## Operational Efficiency & Automation
          - US Bank: Developed new training metrics using Visual Basic, MS Excel, and **ANOVA testing**, which led to a 20% reduction in training time for operational staff.
          - Wells Fargo: Engineered a Visual Basic and Excel application to automate daily tasks, resulting in a **50% reduction in required effort**.
          - Informa: Automated SQL views and stored procedures to ensure data freshness and maintain service level agreements (SLAs), ensuring continuous data availability.
          - Wells Fargo: Implemented an updated FAQ system and **conducted A/B testing** to validate project impact. This effort led to a 15% decrease in overall phone call time by providing consistent and quick information to both customers and internal employees.
      
        - ## Strategic Insights, Research & Mentorship
          - edX (Arizona State University): Served as a Fintech/Data Science instructor for a remote bootcamp. **Taught core concepts including machine learning, predictive analytics**, and blockchain. Mentored students on research projects, providing expertise in experimental design and data pipelines.
          - Informa: Led the design of surveys for the finance industry, which resulted in new services with profit margins of 50%-75%. This work focused on maximizing study value while minimizing resource use.
          - Informa: Integrated third-party data to enrich existing company data through feature engineering, resulting in improved market share approximations and a 10% increase in product valuation.
          - AFCAA: Conducted research on sub-element learning curves and acquisition lag effects in Python within Databricks and Excel. This led to a 10% change in expected R&D costs.
    design:
      columns: '1'
  - block: resume-skills
    content:
      title: Skills & Hobbies
      username: admin
    design:
      show_skill_percentage: false
      columns: 3
  - block: resume-awards
    content:
      title: Certificates
      username: admin
  - block: resume-languages
    content:
      title: Languages
      username: admin
---
