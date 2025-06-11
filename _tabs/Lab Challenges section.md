---
title: Lab Challenges section
layout: page  # Uses Chirpy's card layout
icon: fas fa-laptop-code
order: 4
permalink: /challenges/
---

# 🧪 Lab Challenges

This section showcases key lab challenges I completed as part of the **Cyber Shujaa Program**. These projects reflect my growing proficiency in data handling, exploratory analysis, and web scraping using Python. Each challenge enhanced my technical skillset and introduced me to new tools, libraries, and data problem-solving approaches.

---

## 📊 Titanic Exploratory Data Analysis

**Problem Statement:** 
Perform in-depth Exploratory Data Analysis (EDA) on the Titanic dataset from Kaggle to uncover insights into survival patterns.

**Approach:**
- Initial data profiling using `df.info()`, `df.describe()`, and more.
- Handled missing values using mean, mode, and column removal (e.g., `Cabin`).
- Conducted univariate, bivariate, and multivariate analysis to understand distributions and relationships.
- Applied outlier detection using IQR and Z-score methods.
- Visualized survival patterns based on age, gender, class, and fare.

**Tools & Libraries Used:** 
`Pandas`, `NumPy`, `Seaborn`, `Matplotlib`, `Missingno`

**Visuals & Highlights:**
- KDE plots for survival distribution by age 
- Violin plots for survival by gender and class 
- Mosaic and 3D scatter plots for multivariate interaction

**Key Lessons Learned:**
- Data preprocessing is critical before model building.
- Visualization helps uncover meaningful patterns in survival trends.
- Combining multiple variables (e.g., gender + class) improves insight depth.

📎 [View Notebook on Kaggle](https://www.kaggle.com/code/reaganodhiambootieno/eda-titanic-case-study)

---

## 🌐 Web Scraping & Data Handling in Python

**Problem Statement:** 
Scrape structured data from a public website, clean it, and export it for future analysis.

**Approach:**
- Sent HTTP requests to fetch HTML using `requests`.
- Parsed HTML tables using `BeautifulSoup`.
- Extracted headers and rows, stored them in a `pandas` DataFrame.
- Exported the final structured dataset as a `.csv`.

**Tools & Libraries Used:** 
`requests`, `BeautifulSoup`, `pandas`, Google Colab

**Visuals & Highlights:**
- HTML parsing using tag filters 
- Clean CSV export with index exclusion

**Key Lessons Learned:**
- Web scraping empowers data scientists to access real-world data.
- Understanding HTML DOM structure is essential for efficient scraping.
- Data cleanup after scraping is crucial for analysis readiness.

📎 [View Colab Notebook](https://colab.research.google.com/drive/1aeS4gEijiz7rFSPwKPS-NtkLSm5idATH?usp=sharing)

---

## 🎬 Netflix Data Wrangling

**Problem Statement:** 
Clean and structure the Netflix dataset to address quality issues like missing values and inconsistent data types.

**Approach:**
- Performed data discovery and identified missing or inconsistent entries.
- Converted `date_added` to datetime format and split `duration` into numeric values and units.
- Created mappings to fill missing values using cast-director and director-country relationships.
- Validated and exported a clean dataset ready for modeling.

**Tools & Libraries Used:** 
`pandas`, `datetime`, `NumPy`

**Visuals & Highlights:**
- Null handling using conditional imputation 
- Director-cast pairing logic for inferring missing fields

**Key Lessons Learned:**
- Cleaning is more than just deleting nulls—it’s about inferring context-aware values.
- Transforming features like duration adds analytical flexibility.
- Proper validation ensures dataset integrity and reliability.

📎 [View Notebook on Kaggle](https://www.kaggle.com/code/reaganodhiambootieno/netflix-data-wrangling)

---

> 🔎 These lab challenges reflect my hands-on growth in data science. I’m continuously building projects that showcase real-world applications of data skills. Connect with me for collaborations!
