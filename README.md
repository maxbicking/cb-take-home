# GLUED Analysis
 
This repository contains a Jupyter notebook `GLUED_Analysis.ipynb` that explores the **Global Longitudinal University Enrollment Dataset (GLUED)**. The dataset tracks estimated student counts for roughly 17,000 universities in 194 countries from 1950 to 2020 in five-year intervals. 
 
---
 
## Table of Contents
 
1. **Imports and Data Cleansing** 
    *  Loads `enrollments.csv` and `Countries GDP 1960-2020.csv` directly from CB's public repo
    * Scrubs important columns of unwanted characters and encoding errors
 
2. **Exploratory data analysis (EDA)** 
    * Visualises enrollment trends globally and by region
    * Computes compound annual growth rates (CAGR) to find top 10 fastest-growing countries by total enrollment
 
3. **Difference-in-Differences Causal Case Study - South Africa** 
    * Uses a difference-in-differences (DiD) regression to test whether post-apartheid reforms boosted enrollments 
    * **Result:** point estimate ~ 7,700 students per South-African university per year (95 % CI –2 600 … +18 100)
 
4. **GDP Analysis** 
    * Correlates national GDP (World Bank) with university enrollment 
    * Pearson = 0.68, R Squared = 0.46
 
5. **Conclusion & Next Steps** 
    * Include additional data sources like UN, IMF, and OECD
    * Cluster countries/regions/universities (K-means) to find peer groups 
    * Normalize data for population
 