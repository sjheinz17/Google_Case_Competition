# Google Churn Case Study


# BizGrow Customer Churn: Root Cause Analysis & Recovery Strategy

## Executive Summary

This project investigates a significant spike in Q3 customer churn for **BizGrow**, a SaaS platform. By integrating usage logs and support ticket data, we identified a specific **"Poison Group"**, which we defined as large customers onboarded after July 2023 who were responsible for **80% of total revenue loss**. The analysis revealed a causal link between feature overselling by sales teams and a **27% drop in customer productivity** at the four-month mark, ultimately threatening **$29M in contracts**.

## The Problem

BizGrow experienced an unexpected surge in churn, defined as a non-renewal event following the end of a customer contract.

* **Primary Objective:** Identify the biggest driver of the Q3 churn spike.


* **Revenue Impact:** Approximately $29M in current contracts are at risk due to this churn trend.



## Methodology: Defining the "Poison Group"

To isolate the root cause, we segmented the customer base to find the "Poison Group", which is a minority of customers responsible for the majority of revenue loss.

* **Cohort Criteria:** Companies with **>50 employees** that initiated contracts in **July 2023 or later**.


* **Revenue Correlation:** This specific group accounts for nearly **~80% of revenue loss** attributed to churn.



## Key Insights & Root Cause

The data indicates that churn was not a result of general dissatisfaction, but a specific technical and departmental misalignment.

### 1. Sales-Product Misalignment

* Sales teams were found to be **overselling "multi-warehousing"** as a standard, out-of-the-box feature.


* In reality, multi-warehousing (storing data across multiple warehouses) was not yet stable for high-complexity users.



### 2. The "Four-Month Wall"

* **Productivity Dip:** The Poison Cohort experienced a **27% drop in productivity** (measured by feature events per minute) exactly **four months** into their contract.


* **Technical Trigger:** This dip correlates directly with a spike in support tickets regarding **"bulk upload"** and **"multi-warehouse"** issues.


* **Churn Path:** The unresolved technical issues led to decreased productivity, which served as the primary precursor to churn.



## Strategic Recommendations

I proposed a two-tiered strategy to stabilize the customer base and recover the $29M at risk.

* **Short-term (Sales Training):** Update the sales pitch to localize churn by focusing efforts on customers who do **not** require "Data Warehouse" features until the product stabilizes.


* **Long-term (Product Roadmap):** Pivot the product roadmap to prioritize fixing "Data Warehouse" and "Bulk Upload" stability. This will stop the productivity dip and unlock a new tier of high-value enterprise customers.



## Technical Tools

* **BigQuery:** Used for processing usage logs and merging large-scale datasets across 3,000+ customers.


* **Data Visualization:** Created retention heatmaps and productivity line charts to illustrate the "Poison Cohort" trends.



## Team

* Sanchit Ram Arvind 


* Sammy Heinz 


* Constantin Ertel 


* Nick Fitzpatrick 


* Vineet Reddy

  
* Ray Zhang 
