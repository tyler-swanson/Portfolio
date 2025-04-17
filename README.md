# Swire Coca-Cola Customer Segmentation (IS 6813 | Spring 2025)

## Project Overview
This project was developed as part of the University of Utah’s MSBA Capstone course, in collaboration with a local organization. The objective was to improve customer segmentation between two business models:  
- **Red Truck**: High-volume, high-touch service 
- **White Truck**: Low-volume, third-party distributed service

The existing segmentation strategy relied solely on a 400-unit annual threshold. I developed a data-driven framework to better classify customers by their growth potential and delivery economics.

---

## My Contributions
As an individual contributor to the case competition team, I completed the following:

-  Cleaned and merged data from raw sources into a unified customer-level dataset
-  Performed exploratory data analysis (EDA) with visualizations on order types, customer tenure, delivery costs, and geography
-  Derived new features such as:
  - Return frequency
  - Transaction patterns
-  Developed segmentation logic based on:
  - Customer profile patterns
  - Market signals 
- Forecasted volume, cost, and opportunity loss under both segmentation strategies (rule-based vs 400-unit cutoff)

---

##  Business Impact
- **34% less volume incorrectly routed to White Truck** customers using my segmentation logic
- Potential to reclaim **millions in delivery cost savings**
- Improved resource allocation and labor hours by better targeting Red Truck accounts
- Ensures the organization focuses growth efforts on customers with the *right characteristics*, not just the *highest past volume*

---

## Repo Contents
- `eda_individual_tswanson.Rmd`: My personal exploratory notebook  
- `segmentation_model.Rmd`: My rule-based segmentation logic with strategy comparisons  
- `swire_data_full.Rds`: Enriched dataset used for modeling 
- `README.md`: This file  

---

## Tools & Techniques
- R (`tidyverse`, `gt`, `lubridate`, `leaflet`, `dplyr`)
- Clustering & segmentation
- Cost and opportunity modeling
- Data enrichment and wrangling
- 
---

## Contact
If you'd like to discuss the project or my work in data science and analytics, feel free to reach out on [LinkedIn](https://www.linkedin.com/in/tyler-jacob-swanson).
