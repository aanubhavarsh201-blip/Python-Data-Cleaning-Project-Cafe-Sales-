# ☕ Cafe Sales Data Cleaning Project

## 📌 Project Overview
This project focuses on cleaning and preparing a retail café sales dataset for analysis.  
The dataset contained inconsistent placeholders, missing values, and incorrect data types.

---

## 📂 Dataset
- Raw data: `data/raw/dirty_cafe_sales.csv`
- Cleaned data: `data/cleaned/cleaned_cafe_sales.csv`

---

## 🧹 Data Cleaning Steps

1. Replaced ambiguous placeholders (ERROR, UNKNOWN) with NaN  
2. Converted data types (numeric, datetime, string)  
3. Imputed missing values using business logic:
   - Quantity = Total Spent ÷ Price Per Unit
   - Price Per Unit = Total Spent ÷ Quantity
   - Total Spent = Quantity × Price Per Unit
4. Filled categorical missing values with explicit labels:
   - Unknown Item
   - Unknown Location
   - Unknown Payment Method
5. Removed records with missing Total Spent (0.4% of data)

---

## 📊 Key Data Quality Issues Identified

- Inconsistent placeholders
- Incorrect data types
- Missing financial values
- Incomplete transaction records

---

## ✅ Final Outcome

The dataset is now analysis-ready with:

- Consistent data types
- Valid transaction values
- Transparent handling of missing data
- Minimal data loss

---

## 🛠 Tools Used

- Python
- Pandas
- NumPy
- Jupyter Notebook

---

## 🚀 Future Work

- Exploratory Data Analysis
- Revenue insights
- Dashboard development
