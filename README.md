### 📊 Stack Overflow Developer Survey Trends
Data Cleaning, Imputation & Market Analysis

### 📌 Project Overview

This project analyzes multi-year developer survey data from Stack Overflow to uncover trends in:

🌍 Global developer distribution

🎓 Educational backgrounds

💼 Professional experience

💰 Compensation patterns

The objective was to clean incomplete data, apply statistical imputation techniques, and generate actionable insights about the global developer workforce.

### 🎯 Business Problem

Organizations need to understand:

What educational backgrounds are common among developers?

Is a Computer Science degree still dominant?

How does experience translate into compensation?

What is the “going rate” for developers in today’s market?

This analysis supports workforce planning, salary benchmarking, and talent strategy decisions.

### 📊 Dataset

Multi-year survey responses including:

Variable	Description
Country	Respondent’s country
UndergradMajor	Undergraduate degree major
YearsCodePro	Years of professional coding experience
ConvertedComp	Annual compensation (standardized USD)
DevType	Developer role type

### 🧹 Data Cleaning & Missing Data Strategy

Real-world survey data is rarely complete. This project demonstrates structured handling of missing values.

### 1️⃣ Single Imputation — NOCB

Used for: UndergradMajor

2020 data was complete

Final declared major carried backward

Appropriate because undergraduate major is a fixed historical attribute

### 2️⃣ Multiple Imputation

Used for:

YearsCodePro

ConvertedComp

Iterative imputation (up to 20 iterations)

Leveraged correlation between experience and salary

Preserved distribution integrity

Reduced bias compared to simple mean/median fill

### 📈 Exploratory Data Analysis
#### 🎓 Education Trends

Majority of developers studied Computer Science

Proportion of CS majors declined over time

Suggests increased entry from non-traditional pathways

Insight: Alternative education paths are becoming more viable in tech.

#### 💼 Experience vs Compensation

Boxplot analysis shows:

Positive correlation between experience and salary

High variability at each level

Clear upward compensation trend

Insight: Experience remains a strong predictor of compensation in the developer market.

### 🔍 Key Findings

✔ Developer workforce is globally distributed
✔ Computer Science remains dominant but declining proportionally
✔ Non-CS majors increasingly represented
✔ Experience strongly correlates with compensation
✔ Multiple imputation improves analytical reliability

### 🛠️ Tech Stack

Python

Pandas

NumPy

Matplotlib

Scikit-learn

Jupyter Notebook

### 📁 Project Structure
```bash
stack-overflow-survey-trends/
│
├── data/
│   ├── raw/
│   └── cleaned/
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_imputation.ipynb
│   └── 03_analysis_visualization.ipynb
│
├── images/
│   └── plots/
│
└── README.md
```
### 📊 Skills Demonstrated

Exploratory Data Analysis (EDA)

Data Cleaning & Preprocessing

Missing Data Imputation (Single & Multiple)

Statistical Reasoning

Data Visualization

Business Insight Communication

### 🚀 Future Improvements

Role-based salary modeling

Regional compensation comparison

Predictive salary regression model

Dashboard deployment (Streamlit / Tableau)

### 📎 Conclusion

This project demonstrates the ability to:

Work with messy, real-world datasets

Apply statistically appropriate imputation techniques

Extract meaningful trends

Translate analysis into business-relevant insights
