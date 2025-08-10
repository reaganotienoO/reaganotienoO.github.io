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

# 3. AtliQ Grands Hotel Analytics Dashboard

![Dashboard Screenshot](/assets/projects/hotel_analytics.PNG)  
*Interactive Power BI dashboard for revenue, occupancy, and booking analysis*

---

## Overview

This project delivers a business intelligence solution for **AtliQ Grands**, a luxury hotel chain in India, to address declining market share. Using Power BI, I transformed raw hotel data into actionable insights to support decisions around pricing, occupancy, and revenue management.

🔗 **Live Dashboard**:  
[View in Power BI](https://app.powerbi.com/reportEmbed?reportId=d1f8a079-e99d-4e12-a017-15651d8406a5&autoAuth=true&ctid=c5f7004a-3295-4205-9179-1b0ca576040c)

---

## Business Problem

AtliQ Grands was facing challenges that affected its revenue and competitive standing:

- Ineffective pricing strategies.
- Limited visibility into booking channel performance.
- No centralized tool for real-time performance monitoring.

---

## Solution Highlights

### 1. Data Model (Star Schema)

- **Fact Tables**:
  - `fact_bookings`: revenue, cancellations.
  - `fact_aggregated_bookings`: occupancy.
- **Dimension Tables**:
  - `dim_date`
  - `dim_rooms`
  - `dim_hotel`
- Relationships were defined to support clean filtering and performance.

### 2. Key DAX Metrics

```dax
Revenue = SUM(fact_bookings[revenue_realized])
RevPAR = DIVIDE([Revenue], [Total Capacity])  // Revenue per available room
ADR = DIVIDE([Revenue], [Total Bookings], 0)  // Average Daily Rate
Occupancy % = DIVIDE([Total Successful Bookings], [Total Capacity], 0)
```
### 3. Dashboard Features

**KPIs:**
- Total Revenue: ₹1.76B  
- Occupancy: 57.79%  
- ADR (Average Daily Rate): ₹12,695  

**Filters:**
- City  
- Room Type  
- Week Number  
- Booking Platform  

**Insights:**
- Mumbai properties led in revenue, with ₹84M from AtliQ Enrica.  
- Weekday occupancy was lower (55.85%) compared to weekends (62.64%).  
- Direct bookings had a 70% realization rate, while third-party platforms achieved only 50%.

---

## Tools & Techniques

- **Power BI**: Built interactive visuals, KPIs, and custom DAX measures.  
- **Power Query**: Cleaned and pre-processed data, including fixing incorrect `day_type` values.  
- **Star Schema**: Used to optimize performance and ensure clean relationships between tables.

---

## Key Insights

### Revenue Drivers
- Luxury rooms accounted for 60% of total revenue.
- Hyderabad properties had the highest occupancy rate at 66.07%.

### Booking Channels
- Direct bookings had a higher ADR (₹14,200) than bookings from travel websites (₹11,500).

### Weekly Trends
- Revenue peaked in Week 25 (₹87M), likely due to holiday demand.

---
# 4.California Housing Price Prediction

## Project Overview
This project predicts median house values in California using the California Housing dataset. It implements a complete ML workflow including data preprocessing, KNN regression model training with hyperparameter tuning, evaluation, and deployment via FastAPI.

## Features
- Data preprocessing pipeline with imputation and scaling
- KNeighborsRegressor with GridSearchCV for hyperparameter tuning
- Model evaluation using R², MSE, and RMSE metrics
- FastAPI deployment for real-time predictions

## Technologies Used
- Python
- scikit-learn
- FastAPI
- NumPy, pandas

## Results
Best model achieved:
- R² Score: 0.722
- RMSE: 0.603

## How to Use
1. Clone this repository
2. Install requirements: `pip install -r requirements.txt`
3. Run the FastAPI app: `uvicorn app:app --reload`
4. Send POST requests to `/predict` endpoint with housing features

## Code
[View on Colab](https://colab.research.google.com/drive/1a1DJ0YqranKoRB5cIXm7VeZ7QhizilLq?usp=sharing)

## Future Improvements
- Try other regression algorithms (Random Forest, Gradient Boosting)
- Feature engineering on geographical coordinates
- Add more comprehensive error handling in API



