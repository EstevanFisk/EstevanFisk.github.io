---
title: "Integrated Retail Intelligence: Predictive Operations Control Center on Shiny Dashboards"
summary: "ML-driven pricing & forecasting to end sales bottlenecks and accelerate time-to-close."
date: 2025-12-15
authors:
    - admin
type: project
content_meta:
  content_type: 'App'
links:
  - type: code
    name: GitHub Repo
    url: https://github.com/EstevanFisk/Bike_sales_dashboard_RShiny
    icon: brands/github
  - type: code
    name: Demand Forecasting App Live Demo
    url: "/projects/bike_rshiny_dashboard/demand_app/"
  - type: code
    name: Product Price Prediction App Live Demo
    url: "/projects/bike_rshiny_dashboard/pricing_app/"
tags:
  - R
  - Shiny
  - Feature Engineering
  - Dashboard
  - Timeseries
  - Forecasting
  - Machine Learning
  - SQLite
  - Business Intelligence
  - Regression Analysis
  - Sales Enablement
  - Retail Ops
sitemap: true
share: false
featured: true
build:
  list: always
  render: always
image:
  filename: bikes_rshiny_featured.png
#weight: 10
draft: false
---


This project combines a Demand Forecasting and Customer Analytics Dashboard with a Machine Learning-Driven Product Price Prediction Tool, creating an integrated suite for strategic sales, inventory, and pricing optimization for a bicycle retail business. The solution operationalizes advanced analytics into user-friendly Shiny applications, delivering immediate, data-driven insights to both management and sales teams.


## Demand Forecasting and Customer Analytics Dashboard
This project demonstrates a high-impact, interactive Shiny application designed for rapid sales analysis and predictive demand forecasting within a simulated bicycle retail business. The solution operationalizes advanced analytics into a user-friendly dashboard, providing immediate, actionable insights.

Originally developed as coursework at Business Science University, the application extends core business analysis with robust data science methodologies and a professional-grade user experience (UX).

### Business Value & Impact (For Stakeholders)
The dashboard enables stakeholders to quickly assess market performance, identify sales opportunities, and proactively manage future demand:
- **Strategic Focus**: Rapidly evaluate revenue concentration by geographic market to concentrate sales efforts and optimize resource allocation.
- **Performance Monitoring**: Utilize intuitive health and wealth metrics (e.g., sales above/below $10k, volume thresholds) to flag areas requiring immediate attention or celebrating success.
- **Proactive Planning**: Leverage integrated forecasting capabilities to visualize future trends and hedge against potential opportunities or risks in inventory management and sales targets.
- **Actionable Insights**: Drill down into specific customer segments to understand purchasing behavior and identify upsell potential (e.g., Mountain/Road bike ratio analysis).

### Technical Overview & Methodology (For Data Scientists)
The application leverages a modern R-based tech stack to deliver speed, versatility, and aesthetic appeal:
- Frontend: Developed using the shiny package for reactive web interfaces, enhanced with custom CSS for professional aesthetics (including light/dark themes and dynamic colored indicators).
- Backend & Data Layer: Data is sourced from an SQLite database file. The application manages data parsing and interactivity efficiently.
- Forecasting Methodology: Employs machine learning (ML) models for time-series forecasting, specifically chosen over traditional methods (like ARIMA) to showcase faster performance and greater versatility across various time divisions (daily, weekly, monthly).
- Feature Engineering: The timetk package was utilized to derive extensive time series features for the ML models, significantly boosting real-time prediction performance.
- Visualizations: Includes loess smoothers within time-series plots for localized trend detection and thematic state mapping to visualize revenue density.

### Key Application Features
- Interactive Forecasting: Ability to predict and visualize current and future trends at flexible time intervals.
- Geographic Analysis: A choropleth map visualization of US states shaded by revenue size, highlighting top-performing markets.
- Dynamic Metric Indicators: Visual health metrics for sales volume (Danger/Warning/Healthy zones) and revenue metrics (e.g., under $5K, under $10K, $10K+).
- Customer Segmentation: Mountain-to-Road bike ratio labels used to signal warning zones/upsell potential for specific customer segments.


<a href="/projects/bike_rshiny_dashboard/demand_app/" class="btn btn-primary btn-lg" target="_blank" rel="noopener noreferrer">View Interactive Forecasting Dashboard</a>



## Machine Learning-Driven Product Price Prediction Tool
This project showcases a practical application of machine learning developed to empower sales teams with immediate, accurate pricing capabilities. By providing a self-service tool, it minimizes friction in the sales cycle and streamlines product management workflows.

### Business Value & Impact (For Stakeholders)
As a former Product Manager, I recognized that deal-cycle friction often stems from a lack of immediate, reliable pricing data for sales teams. This tool was engineered to solve that specific inefficiency: 
- **Field-Level Autonomy**: Decouples sales representatives from central pricing teams, providing them with an autonomous, high-fidelity estimation tool to provide quotes in real-time.
- **Operational Throughput**: By automating routine pricing inquiries through ML, product management and pricing specialists can shift focus from "support tickets" to high-level strategic initiatives.
- **Market-Aligned Accuracy**: Utilizes a trained predictive model to ensure new product configurations are priced relative to the existing portfolio, preventing "margin leakage" and ensuring internal price consistency.
- **Accelerated "*Time-to-Close*"**: Eliminating the 24-48 hour wait for pricing approval directly reduces the sales cycle duration and improves the customer experience at the point of sale.

### Technical Overview & Methodology (For Data Scientists)
The application leverages a predictive machine learning model to provide real-time pricing guidance based on existing product data: 
- Core Functionality: The tool allows users to input parameters for a hypothetical new bike model. It utilizes a trained machine learning model to predict an optimal price point based on the existing product portfolio data.
- Interactive Interface: Built with an interactive Plotly graph that visualizes the existing product landscape. The specific predicted price point for the user’s input is dynamically highlighted in green, providing immediate visual context.
- User Input Handling: The application handles user inputs efficiently, requiring standardized formatting (e.g., camel case for model names) to interface correctly with the underlying data model.
- Model Integration: The focus is on operationalizing a machine learning model into a reliable, front-end application that delivers analytical value directly to end-users.

### Key Application Features
- Dynamic Prediction: Predicts prices of new product configurations in real-time based on user-defined feature parameters.
- Interactive Visualization: Uses Plotly for rich, interactive graphing that contextualizes the predicted price within the current market landscape.
- Self-Service Enablement: A user-friendly interface designed specifically for non-technical field personnel.

<a href="/projects/bike_rshiny_dashboard/pricing_app/" class="btn btn-primary btn-lg" target="_blank" rel="noopener noreferrer">View Interactive Price Prediction Dashboard</a>

