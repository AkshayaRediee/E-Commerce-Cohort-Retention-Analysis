# E-Commerce-Cohort-Retention-Analysis
Customer cohort and retention analysis built in Databricks using PySpark and Spark SQL. Customers are grouped into monthly cohorts based on first purchase date, with retention calculated over time. Outputs include retention matrices and Delta tables to support scalable analytics and reporting. 

## Project Overview
This project performs an end-to-end customer cohort and retention analysis using transactional data to understand customer behavior, engagement trends, and churn patterns over time. It mirrors real-world product and data analytics workflows used in e-commerce and subscription-based businesses.

The solution is implemented in a Databricks cloud environment using PySpark and Spark SQL to support scalable, production-style data processing.

---

## Objectives
- Assign customers to monthly cohorts based on first purchase date  
- Measure customer retention over time using months-since-cohort logic  
- Build reusable retention matrices for longitudinal analysis  
- Prepare analytics-ready datasets for dashboards and reporting  

---

## Tech Stack
- Databricks  
- PySpark  
- Spark SQL  
- Delta Lake  
- Python  

---

## Data Processing Workflow
1. Load transactional data into Databricks  
2. Clean and normalize date fields  
3. Identify each customer’s first purchase month  
4. Assign customers to monthly cohorts  
5. Calculate months elapsed since cohort start  
6. Aggregate retained customers by cohort and time period  
7. Generate retention matrices and summary tables  

---

## Key Outputs
- Monthly customer cohort table  
- Retention matrix showing customer activity over time  
- Persisted Delta tables for reproducibility and performance  
- SQL-ready datasets for reporting and KPI analysis  

---

## Business Use Cases
- Customer retention and churn analysis  
- Product and growth analytics  
- Cohort-based KPI tracking  
- Analytics engineering workflows  

---

## Skills Demonstrated
Cohort Analysis, Retention Analysis, PySpark, Spark SQL, Databricks, Delta Lake, Data Cleaning, Analytical SQL, Customer Analytics

---

## Notes
This project is modular and reusable and can be extended for funnel analysis, A/B testing evaluation, and product performance tracking.
