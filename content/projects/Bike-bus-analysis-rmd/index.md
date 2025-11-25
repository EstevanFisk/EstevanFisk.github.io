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
weight: 30
---

This project demonstrates my capability in R by rebuilding a sales analysis dashboard originally developed at [Business Science University](https://www.business-science.io/). The solution uses R-Markdown to present actionable insights into a bicycle company's revenue. For full transparency and technical review, the reports include interactive buttons to review inline code for visibility, allowing readers to inspect the methodology alongside the analysis. The complete project implementation, including all scripts and preliminary model attempts is accessible via my GitHub Repository. This experience was a great refresher on building effective, interactive data visualizations. 

<!--more-->
## Sales Dashboard Example

The core of the dashboard allows users to break down sales by total, category, and time series (quarterly, monthly, or weekly), with additional filtering to analyze specific bicycle types. 

<iframe src="/uploads/notebooks/bike_bus_analysis_rmd/sales_report.html" width="100%" height="1000px" style="border:none;"></iframe>



## Product Analysis Report Example

This portfolio piece addresses a strategic Research and Development (R&D) challenge: benchmarking the existing product line to identify opportunities for new products and optimal pricing. The analysis involved segmentation of the current bicycle inventory, leading to a market gap analysis that revealed viable unserved bicycle combinations. We then utilized machine learning to predict potential price points for the newly identified bicycles based on the features and pricing of existing inventory. Models tested were: linear (with and without regularization), decision tree, random forest, and XGBoost. XGBoost model was ultimately selected as the final predictive solution for its superior performance.

The resulting interactive report enables stakeholders to easily explore the predictive model outputs and review individual data point characteristics for validation.

<iframe src="/uploads/notebooks/bike_bus_analysis_rmd/new_product_recommendation.html" width="100%" height="1000px" style="border:none;"></iframe>


## Customer Segmentation Report

Customer segmentation was conducted using the k-means algorithm on customer sales data. The resulting clusters were then transformed via UMAP techniques into a 2D projection for visualization. Finally, the top 5 bike models were plotted based on customer segment, bike type, and unit price to provide a visual representation of the cluster findings.

<iframe src="/uploads/notebooks/bike_bus_analysis_rmd/customer_segmentation.html" width="100%" height="1000px" style="border:none;"></iframe>


