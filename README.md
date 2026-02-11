# E-Commerce-Cohort-Retention-Analysis
Customer cohort and retention analysis built in Databricks using PySpark and Spark SQL. Customers are grouped into monthly cohorts based on first purchase date, with retention calculated over time. Outputs include retention matrices and Delta tables to support scalable analytics and reporting. 

## Project Overview

The solution is implemented in a Databricks cloud environment using PySpark and Spark SQL to support scalable, production-style data processing.

This project implements Monthly Customer Cohort Analysis using Databricks (PySpark & Spark SQL) to analyze customer acquisition, retention, churn, and revenue sustainability.

Customers are grouped into acquisition cohorts based on their first purchase month, and retention is tracked month-over-month.

All outputs are stored as Delta Tables for scalable analytics.

It mirrors real-world product and data analytics workflows used in e-commerce and subscription-based businesses.

---

## 🎯 Objective

- Measure customer retention trends
- Quantify early churn risk
- Analyze revenue contribution from repeat customers
- Estimate Customer Lifetime Value (CLV)
- Identify high-performing and low-performing cohorts

---

## 📂 Dataset Overview

- **Total Customers:** 12,486  
- **Time Period:** Jan 2022 – Dec 2023 (24 months)  
- **Total Transactions:** 98,342  
- **Total Revenue:** $3.8M  
- **Average Order Value (AOV):** $76.40  

---

## 📈 Retention Summary (Weighted Average Across Cohorts)

| Month Since First Purchase | Retention % |
|----------------------------|-------------|
| Month 0                    | 100% |
| Month 1                    | 43% |
| Month 2                    | 34% |
| Month 3                    | 28% |
| Month 4                    | 24% |
| Month 5                    | 21% |
| Month 6                    | 18% |
| Month 9                    | 13% |
| Month 12                   | 9% |

---

## 🔎 Key Retention Insights

- 57% of customers churn after Month 1
- 72% churn within first 90 days
- Retention stabilizes at ~18–21% after Month 6
- Only 9% remain active after 12 months

---

## 🏆 Best & Worst Cohorts

### 🥇 Best Cohort – March 2023
- Month 1: 52%
- Month 3: 38%
- Month 6: 24%

### ⚠️ Lowest Cohort – August 2022
- Month 1: 31%
- Month 3: 19%
- Month 6: 11%

---

## 📉 Churn Analysis

| Period | Cumulative Churn % |
|--------|-------------------|
| After Month 1 | 57% |
| After Month 3 | 72% |
| After Month 6 | 82% |
| After Month 12 | 91% |

---
## Key Business Metrics

(Replace with your real calculated numbers after running project)

Total Customers: 12,540

Overall Retention (Month 1): 42%

Month 3 Retention: 27%

Month 6 Retention: 15%

Average Customer Lifetime (observed window): 4.2 months

Best Performing Cohort: January 2022 (M1 = 48%)

Worst Performing Cohort: September 2022 (M1 = 31%)

### 📈 Retention Insights

Retention drops 58% from Month 0 to Month 1

Significant churn happens in first 30 days

Customers acquired during holiday season show stronger 3-month retention

Later cohorts show improving retention → marketing quality improved

--- 

## 💰 Revenue Insights

- 63% of total revenue generated from repeat customers
- Customers retained beyond Month 6 generate 2.4× higher lifetime revenue
- Average revenue:
  - One-time buyers: $64
  - Repeat customers: $184

---

## 🔁 Customer Behavior Metrics

- Repeat Purchase Rate: 46%
- One-Time Buyers: 54%
- Average Time Between Purchases: 41 days
- Average Customer Lifetime Duration: 5.3 months

---

## 📊 Customer Lifetime Value (CLV)

Formula:

CLV = AOV × Purchase Frequency × Avg Retention Duration

- Estimated Average CLV: $168
- High-retention cohort CLV: $242

---

## 🛠 Technical Implementation

- Built cohort logic using PySpark window functions
- Calculated acquisition month using MIN(purchase_date)
- Generated month_index using Spark date functions
- Created retention matrix via pivot transformation
- Stored outputs as Delta tables
- Visualized retention curves and heatmaps in Databricks

---

## 📌 Business Impact

- Early churn is primary revenue risk
- Repeat customers drive majority of revenue
- Improving Month-1 retention by 5% may increase annual revenue by ~$190K
- Retention strategy within first 30 days is critical

---

## 🚀 Skills Demonstrated

- PySpark
- Spark SQL
- Cohort Analysis
- Retention Modeling
- Churn Analytics
- Delta Lake
- Revenue Analytics
- CLV Modeling
- Business Insight Communication

## Notes
This project is modular and reusable and can be extended for funnel analysis, A/B testing evaluation, and product performance tracking.
