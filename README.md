# Data-Analysis-Pipeline
# 🧹 Data Cleaning — Ames Housing

This mini project implements a structured data cleaning pipeline for the Ames Housing dataset.

## 🎯 Objectives

The notebook performs the following steps:

- Load dataset using `pd.read_csv()`
- Display first 5 rows
- Check dataset shape
- Inspect data types and fix at least two columns
- Detect missing values
- Handle missing data (median for numeric, mode for categorical)
- Check and remove duplicates
- Detect outliers using boxplot
- Cap extreme `SalePrice` values at the 99th percentile
- Apply final validation checks

## 🔎 Cleaning Decisions

- Numeric columns filled with median to reduce impact of skew and outliers
- Categorical columns filled with mode to preserve most frequent category
- Feature-absence columns filled with `"None"`
- Outliers capped instead of removed to avoid data loss

## ✅ Validation Checks

The pipeline ensures:

- No null values in `SalePrice`
- All `SalePrice` values are positive
- Dataset is not empty after cleaning

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib

## 📦 Output

The `clean_data()` function returns a cleaned dataset ready for further modeling and analysis.
