# Swire Coca-Cola Capstone Project – Delivery Optimization - Individual Work

**Tyler Swanson**  
[LinkedIn Profile](https://www.linkedin.com/in/tyler-jacob-swanson)

---

## Project Overview

This project was completed as part of the **IS 6813 – Analytics Capstone** at the University of Utah, in partnership with **Swire Coca-Cola**. The goal was to **optimize customer segmentation for beverage delivery**, improving operational efficiency and identifying high-growth customers using advanced analytics.

Swire currently delivers via two service models:
- **Red Truck**: In-house delivery for high-volume accounts
- **White Truck**: 3rd-party delivery for smaller, less profitable accounts

We proposed a smarter, data-driven delivery assignment strategy by:
- Predicting customer value using characteristics **not reliant on volume**
- Improving assignment to Red or White Truck to **reduce cost and recapture future growth**

---

## Business Value

✔️ **Cost Optimization**: Reassignment of low-potential accounts from Red to White Truck frees up high-cost labor and delivery routes  
✔️ **Growth Enablement**: Retains high-potential customers under Red Truck to increase sales velocity  
✔️ **Data-Driven Strategy**: Uses machine learning to prevent reliance on rigid volume thresholds  
✔️ **Future-Proof**: Incorporates channel type and market conditions into decisioning

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| `Tyler_Cleaning_Script.Rmd` | Full cleaning pipeline – reads, merges, and standardizes data for modeling |
| `Modeling_Swire_Capstone_Tyler.Rmd` | Individual modeling notebook: clustering, classification, feature importance |
| `README.md` | This page – project summary and value proposition |
| `swire-banner.png` | Optional graphic for repo branding (if desired) |

---

## Technical Highlights

### Data Wrangling
- Cleaned and merged 4 disparate datasets (customer profiles, addresses, transactions, delivery costs)
- Converted delivery ranges, resolved missing zip codes, and parsed geographic metadata
- Removed duplicate transactions and handled negative deliveries (returns)

### Segmentation Strategy
- Applied **PAM Clustering with Gower’s Distance** to assign customers to behavior-based clusters
- Used **KNN and Centroid Matching** to assign missing cluster labels

### Predictive Modeling
- Built **Random Forest classifiers** to predict high-value customers at various thresholds (`400+`, `500+`, `600+` cases/gallons)
- Applied **SMOTE oversampling** to balance the target variable
- Created a dedicated model for **Local Market Partners (LMPs)**

### Model Performance
- Accuracy: ~90%
- Sensitivity: 72–78% for high-value class
- Top Predictors: Customer tenure, cluster, sub trade channel, order type, neighbor transaction behavior

---

## Interview Talking Points

- How I used **unsupervised clustering to uncover latent customer segments**
- Why I focused on **features unrelated to volume** for identifying growth opportunities
- The logic and impact of **reassigning delivery models** using predictive insights
- How I applied **SMOTE** to resolve class imbalance in real-world business datasets
- My process for ensuring **reproducibility and data integrity** throughout the project

---

## How to Run

1. Clone this repo  
2. Open `Tyler_Cleaning_Script.Rmd` to run the full cleaning process  
3. Use the cleaned `Swire_Master_Data` to explore modeling via `Modeling_Swire_Capstone_Tyler.Rmd`  
4. Optional: export visuals or extend with Shiny/Power BI dashboards

---

## Tools Used

- **R (tidyverse, janitor, lubridate, cluster, smotefamily)**
- **R Markdown** for reproducible analysis
- **GitHub** for version control and portfolio building

---

## Connect

I'm passionate about using data to drive business decisions and operational efficiency. If you're looking for a data-driven problem solver with business acumen and technical skills, I’d love to chat.
💼 [LinkedIn](https://www.linkedin.com/in/tyler-jacob-swanson)

---
