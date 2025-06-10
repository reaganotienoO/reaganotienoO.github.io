---
title: Projects section
layout: page
icon: fas fa-project-diagram  # Font Awesome project icon
order: 3  # Adjust based on your navigation order
---

# 1. Healthcare Data Analysis Project

![Dashboard Screenshot](/assets/projects/health.PNG)  

## Overview
This project analyzes healthcare data to uncover trends in patient demographics, hospital admissions, financial performance, and disease prevalence. The goal is to provide actionable insights for improving patient care, optimizing resources, and reducing costs. The analysis was conducted using Excel for data cleaning and exploration, and Power BI for interactive visualization.

## Objectives
- **Patient Demographics**: Analyze age, gender distribution, and common medical conditions.
- **Hospital Admissions**: Examine trends in admissions, length of stay, and seasonal variations.
- **Financial Performance**: Assess total billing, cost drivers, and high-cost conditions.
- **Disease Prevalence**: Identify common chronic diseases and their impact on healthcare costs.
- **Recommendations**: Develop strategies to optimize patient management and reduce costs.

## Tools Used
- **Excel**: Data cleaning, standardization, and preliminary analysis.
- **Power BI**: Interactive dashboard for visualization and deeper insights.

## Key Insights
### Patient Demographics
- **Total Patients**: 55,000 (50.02% Male, 49.98% Female).
- **Age Groups**: Young adults and senior adults dominate the patient population.

### Hospital Admissions
- **Seasonal Trends**: Spikes in admissions during January and July.
- **Length of Stay**: Average of 15 days, with older patients staying longer.

### Financial Performance
- **Total Billing**: \$1 Billion.
- **High-Cost Conditions**: Diabetes and obesity account for nearly \$500M in billing.

### Disease Prevalence
- **Common Conditions**: Diabetes, hypertension, obesity, and arthritis are prevalent, especially among older patients.

## Recommendations
1. **Preventive Care**: Implement targeted health programs for young and senior adults to reduce chronic diseases.
2. **Cost Optimization**: Invest in preventive measures and negotiate better insurance coverage for chronic conditions.
3. **Resource Management**: Increase staffing during peak months and introduce home-based care programs to optimize bed usage.
4. **Data-Driven Strategies**: Use predictive analytics for early intervention and personalized treatment plans.

## Interactive Dashboard

Explore the full analysis in the interactive Power BI dashboard:  
[View Dashboard](https://app.powerbi.com/reportEmbed?reportId=c9e08f52-3df8-4e35-a979-1e7e3b536430&autoAuth=true&ctid=c5f7004a-3295-4205-9179-1b0ca576040c)

## Conclusion
This project highlights the power of data analytics in healthcare, offering actionable insights to improve patient outcomes and operational efficiency. The Power BI dashboard enables real-time decision-making for healthcare administrators.

# 2. Netflix Data Wrangling Project

This project demonstrates data wrangling techniques applied to the Netflix dataset available on Kaggle. The goal was to clean, structure, and prepare the data for further analysis or visualization.

## Overview

The dataset contains information about Netflix content, including titles, genres, cast, directors, and release information. The raw dataset had several quality issues, such as missing values, duplicates, and inconsistent formatting. This project focuses on identifying and resolving those issues using Python and pandas.

## Key Objectives

- Load and explore the dataset.
- Identify and fix missing values and duplicates.
- Transform columns to structured formats.
- Extract and enrich features.
- Validate the integrity of the cleaned dataset.
- Export a clean version for downstream use.

## Steps Performed

### 1. Dataset Exploration
- Loaded the data into a pandas DataFrame.
- Examined column types, null values, and checked for duplicate records.
  ![Data Exploration Dashboard](/assets/projects/Data%20exploration.PNG)  

### 2. Structuring the Data
- Converted `date_added` to datetime format.
- Split the `duration` column into numeric values and time units (e.g., minutes vs. seasons).
- Differentiated between movies and TV shows more clearly.

### 3. Cleaning
- Removed duplicates and dropped the unnecessary `description` column.
- Built a mapping of frequent `director-cast` pairs to fill missing `director` fields.
- Used known `director-country` relationships to infer missing country values.
- Filled missing `cast` entries with `"Not Given"`.
- Dropped rows where critical fields like `date_added`, `rating`, or `duration` were missing.

### 4. Error Checking
- Ensured that `date_added` wasn’t earlier than the `release_year`, which would be inconsistent.
- Reviewed and corrected records with logic errors in date fields.

### 5. Final Validation
- Verified that no critical fields had missing values.
- Confirmed all column types were correct.
- Reset the DataFrame index and validated the structure.

### 6. Export
- Saved the cleaned dataset as `cleaned_netflix.csv` for use in further analysis or modeling.

## Tools Used

- Python
- pandas
- Jupyter Notebook

## Result

The final dataset is clean, logically consistent, and ready for analysis. It can now be used for tasks like:
- Trend analysis over time
- Genre and country-based filtering
- Network visualizations of actor-director collaborations

## Project Link

Full code and notebook available on Kaggle:  
👉 [Netflix Data Wrangling on Kaggle](https://www.kaggle.com/code/reaganodhiambootieno/netflix-data-wrangling)

---

Feel free to fork or clone the project if you're interested in building visualizations or running additional analysis on the cleaned data.




