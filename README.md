# Capstone Project – Delivery Optimization (Individual Work)

**Tyler Swanson**  
[LinkedIn Profile](https://www.linkedin.com/in/tyler-jacob-swanson)

---

## Project Overview

This project was completed as part of the **IS 6813 – Analytics Capstone** at the University of Utah in collaboration with **Swire Coca-Cola**. The objective was to develop a smarter delivery strategy by improving how customers are assigned to delivery models (Red Truck vs White Truck), based on their behavioral attributes rather than static volume thresholds.

---

## Business Problem

Swire Coca-Cola uses two delivery models:

- **Red Truck**: In-house service for large, high-volume customers  
- **White Truck**: Outsourced delivery for lower-volume customers  

The current segmentation depends heavily on past order volume (e.g., 400-case thresholds), which fails to capture customer growth potential or market context. This approach risks under-serving emerging high-value customers and misallocating high-cost delivery resources.

---

## Group Solution

Our group proposed a **data-driven segmentation and delivery assignment strategy** by:

- Clustering customers using profile data to uncover behavioral patterns  
- Predicting customer value using classification models not reliant on volume  
- Assigning Red or White Truck status to maximize long-term growth while minimizing unnecessary delivery costs

This method enabled more dynamic and informed delivery decisions based on customer type, tenure, channel, and location.

---

## My Individual Contribution

I contributed to the data pipeline, clustering logic, and predictive modeling:

- **Developed the full cleaning pipeline** in `Tyler_Cleaning_Script.Rmd` to merge and standardize raw data from customer profiles, addresses, transactions, and delivery costs  
- **Applied PAM Clustering** using Gower’s Distance to assign customers to behavior-based groups  
- **Engineered Random Forest classification models** to predict high-value customers at thresholds of 400+, 500+, and 600+ cases/gallons  
- **Handled class imbalance using SMOTE** and evaluated key drivers of customer value  
- **Defined logic for delivery model reassignment** based on predicted customer potential and local market attributes

---

## Business Value

- **Cost Optimization**: Redirected low-potential accounts from Red to White Truck to reduce delivery labor and route costs  
- **Growth Enablement**: Retained high-potential and emerging customers under Red Truck to support future sales  
- **Flexible Strategy**: Accounted for trade channels, tenure, and neighbor behavior in decision-making  
- **Data-Driven Insights**: Provided an explainable, scalable alternative to manual volume-based thresholds

---

## Challenges Encountered

- **Missing Cluster Labels**: Solved using KNN and centroid matching to fill gaps  
- **Noisy Data**: Transaction tables contained returns, duplicates, and zero-volume entries, which required aggressive cleaning  
- **Imbalanced Classification**: Resolved with SMOTE oversampling to improve model sensitivity to high-value customers

---

## Key Learnings

- Customer value can be predicted using traits unrelated to volume  
- Model explainability is critical to business adoption  
- Strong data cleaning lays the foundation for accurate modeling  
- Iterative testing and validation are essential in real-world analytics

---

## Repository Contents

| File | Description |
|------|-------------|
| `EDA.Rmd` | Exploratory Data Analysis (EDA) notebook – investigates patterns in customer profiles and transactions, visualizes key metrics, and identifies trends that inform modeling decisions |
| `Tyler_Cleaning_Script.Rmd` | Full cleaning pipeline – reads, merges, and standardizes data for modeling |
| `Modeling_Swire_Capstone_Tyler.Rmd` | Individual modeling notebook: clustering, classification, feature importance |
| `README.md` | This page – project summary, individual contributions, and business impact of the solution |

---


