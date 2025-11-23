---
title: Bicycle Business Analysis Using R-Markdown
date: 2025-11-10
links:
  - type: site
    name: GitHub Repo
    url: https://github.com/EstevanFisk/bike_business_analysis_rmarkdown
tags:
  - R
  - R-Markdown
  - Dashboard
  - Prediction
  - Feature Engineering
sitemap: true
share: false
---

This project demonstrates my capability in R by rebuilding a sales analysis dashboard originally developed at [Business Science University](https://www.business-science.io/). The solution uses R-Markdown to present actionable insights into a bicycle company's revenue. The core of the dashboard allows users to break down sales by total, category, and time series (quarterly, monthly, or weekly), with additional filtering to analyze specific bicycle types. This experience was a great refresher on building effective, interactive data visualizations.

## Dashboard Example (clean with no code showing)
<iframe src="/uploads/notebooks/bike_bus_analysis_rmd/no_code_sales_report.html" width="100%" height="1000px" style="border:none;"></iframe>

This portfolio piece addresses a strategic Research and Development (R&D) challenge: benchmarking the existing product line to identify opportunities for new products and optimal pricing. The analysis involved segmentation of the current bicycle inventory, leading to a market gap analysis that revealed viable unserved bicycle combinations. We then utilized machine learning to predict potential price points for the newly identified bicycles based on the features and pricing of existing inventory. The resulting interactive report enables stakeholders to easily explore the predictive model outputs and review individual data point characteristics for validation.

## Report Example (clean with no code showing)
<iframe src="/uploads/notebooks/bike_bus_analysis_rmd/no_code_new_product_recommendation.html" width="100%" height="1000px" style="border:none;"></iframe>

For full transparency and technical review, the reports include inline code visibility, allowing readers to inspect the methodology alongside the analysis. The complete project implementation, including all scripts and preliminary model attempts, is accessible via my [GitHub Repository]. Note that after evaluating multiple approaches, the XGBoost model was ultimately selected as the final predictive solution for its superior performance.

## Dashboard Example (with code showing)
<iframe src="/uploads/notebooks/bike_bus_analysis_rmd/with_code_sales_report.html" width="100%" height="1000px" style="border:none;"></iframe>

## Report Example (with code showing)
<iframe src="/uploads/notebooks/bike_bus_analysis_rmd/with_code_new_product_recommendation.html" width="100%" height="1000px" style="border:none;"></iframe>