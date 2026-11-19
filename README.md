# Olist-Ecommerce-Funnel-Analysis
Power BI dashboard analyzing order fulfilment and regional delivery performance for Olist, a Brazilian e-commerce marketplace.
E-Commerce Logistics & Fulfilment Performance

An interactive Power BI dashboard analysing the order fulfilment funnel of Olist, a Brazilian e-commerce marketplace. It tracks how orders move from purchase to approval, shipping and delivery, and compares delivery performance across Brazilian states.

Dashboard preview

Executive Summary

This dashboard analyses the order fulfilment funnel of Olist, covering orders placed between September 2016 and October 2018. It shows how many orders make it through each stage and where delivery performance falls short.

Key findings

The funnel is healthy. Of roughly 99K orders placed, 99.8% were approved, 98.4% were shipped and 98.8% were delivered. About 96K orders (around 97% of those purchased) reached the customer.
Approval is not the bottleneck. Almost every order clears approval, so the small losses occur at the shipping and delivery stages.
Delivery performance varies by region. Most states deliver between 97% and 99.6% of orders. Mato Grosso do Sul (MS), Paraná (PR) and Minas Gerais (MG) are among the strongest.
Roraima (RR) is the clear outlier. Its delivery rate is 91.1%, about 7 percentage points below the 98.8% overall rate and the lowest of any state. Ceará (CE) is next lowest at 97.0%.

Recommendation: Prioritise delivery improvements in Roraima, for example by reviewing carrier coverage and delivery times for that region, since it is the only state well below the rest of the network.

Key Metrics
Metric	Result
Order approval rate	99.8%
Shipping rate	98.4%
Delivery rate	98.8%
Business Questions
What share of orders move through each stage of the funnel?
Where do orders drop off between purchase and delivery?
Which states have the weakest delivery performance?
Dataset
Source: Brazilian E-Commerce Public Dataset by Olist (Kaggle)
Tables used: 8 of the 9 files
Not used: the geolocation table, since the analysis works at state level and does not need map coordinates
Period covered: 4 September 2016 to 17 October 2018
Tools
Power BI Desktop for data modelling, DAX measures and visuals
Kaggle for the dataset
Approach
Loaded the 8 tables into Power BI and checked data types.
Built relationships between the tables in the model view.
Created DAX measures for the approval, shipping and delivery rates.
Designed the Funnel Overview page with KPI cards, a fulfilment funnel, a delivery-rate-by-state chart, and state and date filters.
Dashboard Features
KPI cards for approval, shipping and delivery rates
Order fulfilment funnel from purchase to delivery
Delivery rate by state, ranked from lowest to highest
Slicers for customer state and date range

Note: the funnel and state charts use truncated axes to make small differences visible, so the gaps look larger than they are in absolute terms.

Repository Structure
olist-ecommerce-funnel-analysis/
├── README.md
├── images/
│   └── dashboard-preview.png
└── olist-funnel-analysis.pbix

The raw data is not included. Download it from the Kaggle link above.

How to Open the Dashboard
Download olist-funnel-analysis.pbix from this repository.
Open it in Power BI Desktop (free, Windows only).
If prompted, point the data sources to your own download of the Kaggle files.
Author

Fechi Iroegbu LinkedIn | GitHub
