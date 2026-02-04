# Subscription Churn Analysis

## Why I Did This
This project started as part of my **DataCamp Data Analyst certification**, but I treated it like a **real business problem**.

The company (**Fit.ly**) was losing users, and the churn rate was high enough that it would eventually hurt revenue if nothing changed.  

The goal wasn’t to build a complex model — it was to **understand why users were leaving** and what the business could realistically do about it.

---

## The Data
I worked with **three datasets**:

- **Account data** – customer plans, pricing, churn status  
- **Customer support data** – tickets, topics, resolution times  
- **User activity data** – how often users actually engaged with the product  

Before any analysis, I cleaned and validated the data to ensure reliability. For example:

- Standardized customer IDs so tables could be merged  
- Treated missing churn values as active users, based on product notes  
- Discovered that a column labeled `state` in the support data was actually a **ticket resolution flag**, not a location  

---

## What I Looked For
I focused on questions a **business team would actually ask**:

- Are churned users behaving differently from retained users?  
- Does customer support experience affect churn?  
- Which subscription plans are most at risk?  
- What early signals suggest a customer might leave?  

---

## Key Findings
A few things stood out clearly:

- **High churn rate** – 28.5%, which is not sustainable for a subscription business  
- **Support resolution time matters**:  
  - Retained users waited **~6 hours** on average  
  - Churned users waited **~18 hours**  
- **Engagement is a strong signal** – users who churned barely used the product  
- **Free plan users churn the most**, especially when they experience billing or technical issues  

> In short: people aren’t leaving randomly — they’re leaving after poor early experiences.

---

## Business Recommendations
If this were a real company, I would recommend:

1. Set an **8-hour SLA** for billing and technical support tickets  
2. Add **early engagement nudges** for new users who go inactive  
3. Treat **billing issues as high-priority churn risks**  
4. Move **Free users to paid plans earlier** to increase commitment  

---

## Tools Used
- **Python** (pandas, numpy, matplotlib)  
- **Jupyter Notebook**  
- **Excel** (for initial inspection and validation)  
