# E-Commerce Logistics & Fulfilment Performance

An interactive Power BI dashboard analysing the order fulfilment funnel of Olist, a Brazilian e-commerce marketplace. It tracks how orders move from purchase to approval, shipping and delivery, and compares delivery performance across Brazilian states.

![Dashboard preview](images/dashboard-preview.png)

---

## Executive Summary

This dashboard analyses the order fulfilment funnel of Olist, covering orders placed between **September 2016** and **October 2018**. It shows how many orders make it through each stage and where delivery performance falls short.

### Key Findings

**1. The funnel is healthy**

99.8% of roughly 99K orders were approved, 98.4% were shipped and 98.8% were delivered. About 96K orders (around 97% of those purchased) reached the customer.

**2. Approval is not the bottleneck**

Almost every order clears approval, so the small losses happen at the shipping and delivery stages.

**3. Delivery performance varies by region**

Most states deliver between 97% and 99.6% of orders. Mato Grosso do Sul (MS), Paraná (PR) and Minas Gerais (MG) are among the strongest.

**4. Roraima (RR) is the clear outlier**

Its delivery rate is 91.1%, about 7 percentage points below the 98.8% overall rate and the lowest of any state. Ceará (CE) is next lowest at 97.0%.

### Recommendation

**Prioritise delivery improvements in Roraima.** Review carrier coverage and delivery times for that region, since it is the only state well below the rest of the network.

---

## Key Metrics

| Metric | Result |
|---|---|
| **Order approval rate** | 99.8% |
| **Shipping rate** | 98.4% |
| **Delivery rate** | 98.8% |

---

## Business Questions

**1. Funnel flow:** What share of orders move through each stage of the funnel?

**2. Drop-off points:** Where do orders drop off between purchase and delivery?

**3. Regional gaps:** Which states have the weakest delivery performance?

---

## Dataset

**Source:** [Brazilian E-Commerce Public Dataset by Olist (Kaggle)](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

**Tables used:** 8 of the 9 files

**Not used:** the geolocation table, since the analysis works at state level and does not need map coordinates

**Period covered:** 4 September 2016 to 17 October 2018

---

## Tools

**Power BI Desktop:** data modelling, DAX measures and visuals

**Kaggle:** source of the dataset

---

## Approach

**1. Load the data:** Loaded the 8 tables into Power BI and checked data types.

**2. Build the model:** Created relationships between the tables in the model view.

**3. Write the measures:** Created DAX measures for the approval, shipping and delivery rates.

**4. Design the dashboard:** Built the Funnel Overview page with KPI cards, a fulfilment funnel, a delivery-rate-by-state chart, and state and date filters.

---

## Dashboard Features

**KPI cards:** approval, shipping and delivery rates at a glance

**Order fulfilment funnel:** purchase to delivery, stage by stage

**Delivery rate by state:** ranked from lowest to highest

**Slicers:** filter by customer state and date range

> **Note:** the funnel and state charts use truncated axes to make small differences visible, so the gaps look larger than they are in absolute terms.


