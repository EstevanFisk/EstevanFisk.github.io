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
          - {{< spoiler text="Chipotle Mexican Restaurant (CSUF):NLP Model" >}}Developed an NLP model (Python/Streamlit) to analyze internal and external unstructured text, achieving 90% accuracy in automated comment tagging.
          {{< /spoiler >}}
          - {{< spoiler text="Informa: Demand Elasticity Moodel" >}}Created demand elasticity and propensity-to-buy models (R/R-Shiny), achieving 85% accuracy for sales and marketing strategy insights.{{< /spoiler >}}
          - {{< spoiler text="DCMA: Forecasting Metrics" >}}Designed and evaluated new DOD forecasting metrics using Brier scoring (R, R-Shiny, Power BI), impacting $5.8 trillion in agency contracts.{{< /spoiler >}}
          - {{< spoiler text="Wells Fargo: Workflow Time Series" >}}Conducted a time series analysis in Python to forecast future workflow growth, leading to savings of over 250 overtime hours per month.{{< /spoiler >}}
          - {{< spoiler text="AFCAA: Regression Analysis" >}}Performed regression-based cross-check analysis (Python/Dataiku) on follow-on acquisition costs, leading to a 15% correction of estimated ground costs.{{< /spoiler >}}

        - ### Operational Efficiency & Automation
          - {{< spoiler text="US Bank: Training Reduction" >}}Developed new department training metrics using VBA/Excel and ANOVA testing, resulting in a 20% reduction in training time for staff.{{< /spoiler >}}
          - {{< spoiler text="Wells Fargo: Task Automation" >}}Engineered a Visual Basic and Excel application to automate daily tasks, resulting in a 50% reduction in required effort.{{< /spoiler >}}
          - {{< spoiler text="Informa: SQL Automation" >}}Automated SQL views and stored procedures to ensure continuous data freshness and maintain strict Service Level Agreements (SLAs).{{< /spoiler >}}
          - {{< spoiler text="Wells Fargo: A/B Testing" >}}Implemented a new FAQ system and used A/B testing to validate project impact, decreasing overall phone call time by 15%.{{< /spoiler >}}
      
        - ### Strategic Insights, Research & Mentorship
          - {{< spoiler text="edX (Arizona State University): Research Mentorship" >}}Provided expert mentorship on student research projects, focusing on **experimental design** and optimizing complex data pipelines.{{< /spoiler >}}
          - {{< spoiler text="Informa: Research Design" >}}Led the design of finance industry surveys, resulting in new services with high 50%-75% profit margins.{{< /spoiler >}}
          - {{< spoiler text="Informa: Product Development/Feature Engineering" >}}Integrated third-party data using feature engineering, resulting in improved market share approximations and a 10% increase in product valuation.{{< /spoiler >}}
          - {{< spoiler text="AFCAA: Learning Curve Research" >}}Conducted research on sub-element learning curves and acquisition lag (Python/Databricks), resulting in a 10% change in expected R&D costs.{{< /spoiler >}}
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
