---
title: Lab Challenges section
layout: archive  # Uses Chirpy's card layout
icon: fas fa-laptop-code
order: 4
permalink: /challenges/
---

## 🧪 Data Science & AI Lab Challenges

### 🎬 Netflix Data Wrangling Project
**Cyber Shujaa Program | May 2025**  
**Stack:** Python, Pandas, Kaggle | [View Notebook](https://www.kaggle.com/code/reaganodhiambootieno/netflix-data-wrangling)

#### 📌 Problem Statement
Cleaned a messy Netflix dataset (8,800+ records) containing:
- 29% missing values in critical columns (director, cast, country)
- Inconsistent datetime formats (`date_added`)
- Logical errors between `release_year` and `date_added` fields
- Mixed units in `duration` (minutes vs seasons)

#### 🛠️ Technical Approach
1. **Data Discovery**:
   ```python
   # Identify data quality issues
   print(f"Missing values:\n{df.isnull().sum()}")
   print(f"Duplicates: {df.duplicated().sum()}")
