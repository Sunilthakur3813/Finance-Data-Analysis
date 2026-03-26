# 📊 Credit Lending Analysis

## 🔍 Overview
This project analyzes credit lending patterns by integrating internal bank data with CIBIL datasets. The goal is to clean, merge, and analyze data to generate insights that support loan approval decisions and credit risk management.

---

## 🎯 Objective
- Analyze customer credit profiles  
- Identify patterns in lending behavior  
- Support data-driven loan approval decisions  
- Highlight potential credit risks  

---

## ⚙️ Project Workflow
- Loaded and explored datasets (Bank Internal & CIBIL)  
- Cleaned data by handling missing values and inconsistencies  
- Merged datasets to create a unified customer credit profile  
- Performed data transformations for analysis readiness  
- Conducted exploratory data analysis (EDA)  
- Visualized key patterns using charts  

---

## 🛠 Tech Stack
- **Python (Jupyter Notebook)**  
- **Pandas, NumPy** – Data Cleaning & Manipulation  
- **Matplotlib** – Data Visualization  
- **Excel** – Dataset Source  

---

## 📊 Key Analysis
- Credit Score Distribution  
- Loan Amount vs Credit Score Relationship  
- Identification of missing and inconsistent data patterns  
- Customer-level financial behavior analysis  

---

## 📈 Key Insights
- Customers with higher credit scores tend to receive larger loan amounts  
- Missing data patterns highlight potential data quality issues  
- Credit score distribution shows variation in customer risk levels  
- Strong relationship observed between creditworthiness and lending decisions  

---

## 📷 Visualizations
(Add your screenshots here)

---

## 💻 Sample Code
```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

bank_data = pd.read_excel("case_study1.xlsx")
cibil_data = pd.read_excel("case_study2.xlsx")

merged_df = pd.merge(bank_data, cibil_data, on="Customer_ID", how="inner")
merged_df.fillna(0, inplace=True)

merged_df['Credit_Score'].hist(bins=20)
plt.show()


## 🚀 Outcome
Successfully transformed raw financial data into meaningful insights, demonstrating strong skills in data cleaning, data integration, exploratory analysis, and visualization.
