Credit Lending Analysis

This project analyzes credit lending patterns by combining internal bank data with CIBIL datasets. 
The objective is to clean, integrate, and visualize data to support better loan approval decisions and credit risk management.

# Project Workflow

Loaded and explored datasets (Bank Internal & CIBIL)

Removed null/missing values and standardized fields

Merged datasets to create a unified credit profile

Performed data transformations for consistency

Visualized patterns using Matplotlib

Tools & Libraries

Python (Jupyter Notebook)

Pandas, NumPy – Data Cleaning & Manipulation

Matplotlib – Data Visualization

Excel – Raw Dataset Format

Sample Code
# Import libraries
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

# Load datasets
bank_data = pd.read_excel("case_study1.xlsx")
cibil_data = pd.read_excel("case_study2.xlsx")

# Preview data
print(bank_data.head())
print(cibil_data.head())

# Merge datasets
merged_df = pd.merge(bank_data, cibil_data, on="Customer_ID", how="inner")

# Handle missing values
merged_df.fillna(0, inplace=True)

# Summary statistics
print(merged_df.describe())

# Credit Score Distribution
plt.figure(figsize=(8,5))
merged_df['Credit_Score'].hist(bins=20, color="skyblue", edgecolor="black")
plt.title("Credit Score Distribution")
plt.xlabel("Credit Score")
plt.ylabel("Frequency")
plt.show()

# Loan Amount vs Credit Score
plt.figure(figsize=(8,5))
plt.scatter(merged_df['Credit_Score'], merged_df['Loan_Amount'], alpha=0.5)
plt.title("Loan Amount vs Credit Score")
plt.xlabel("Credit Score")
plt.ylabel("Loan Amount")
plt.show()

# Key Outcomes

Cleaned and merged datasets for accurate analysis

Identified gaps and missing patterns in credit data

Visualized customer credit trends and lending risks

Delivered insights useful for loan decision-making

