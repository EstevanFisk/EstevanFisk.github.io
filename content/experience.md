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
      title: 'Data Science Solutions & Business Impact Projects'
      text: |
        - ### Predictive Modeling & Advanced Analytics
          - {{< spoiler text="Chipotle Mexican Restaurant (CSUF):NLP model" >}}Chipotle Mexican Restaurant (CSUF): Developed an NLP model (Python/Streamlit) to analyze internal and external unstructured text, achieving 90% accuracy in automated comment tagging.
          {{< /spoiler >}}
          - Chipotle Mexican Restaurant (CSUF): Developed an NLP model (Python/Streamlit) to analyze internal and external unstructured text, achieving 90% accuracy in automated comment tagging.
          - Informa: Created demand elasticity and propensity-to-buy models (R/R-Shiny), achieving 85% accuracy for sales and marketing strategy insights.
          - DCMA: Designed and evaluated new DOD forecasting metrics using Brier scoring (R, R-Shiny, Power BI), impacting $5.8 trillion in agency contracts.
          - Wells Fargo: Conducted a time series analysis in Python to forecast future workflow growth, leading to savings of over 250 overtime hours per month.
          - AFCAA: Performed regression-based cross-check analysis (Python/Dataiku) on follow-on acquisition costs, leading to a 15% correction of estimated ground costs.

        - ### Operational Efficiency & Automation
          - US Bank: Developed new department training metrics using VBA/Excel and ANOVA testing, resulting in a 20% reduction in training time for staff.
          - Wells Fargo: Engineered a Visual Basic and Excel application to automate daily tasks, resulting in a 50% reduction in required effort.
          - Informa: Automated SQL views and stored procedures to ensure continuous data freshness and maintain strict Service Level Agreements (SLAs).
          - Wells Fargo: Implemented a new FAQ system and used A/B testing to validate project impact, decreasing overall phone call time by 15%.
      
        - ### Strategic Insights, Research & Mentorship
          - edX (Arizona State University): Provided expert mentorship on student research projects, focusing on **experimental design** and optimizing complex data pipelines.
          - Informa: Led the design of finance industry surveys, resulting in new services with high 50%-75% profit margins.
          - Informa: Integrated third-party data using feature engineering, resulting in improved market share approximations and a 10% increase in product valuation.
          - AFCAA: Conducted research on sub-element learning curves and acquisition lag (Python/Databricks), resulting in a 10% change in expected R&D costs.
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
