# 📊 Credit Customers Data Cleaning using Pandas

## 📌 Project Overview
This project focuses on cleaning and preparing a credit customer dataset using Pandas. The objective is to transform raw data into a structured and analysis-ready format by performing essential data preprocessing steps.

---

## 📂 Dataset Information
- Dataset: Credit Customers Data  
- Rows: 1000  
- Columns: 21 (initially)

---

## 🚀 Data Cleaning Steps

### 1. Data Loading
The dataset was loaded into a Pandas DataFrame for processing and analysis.

---

### 2. Exploratory Data Analysis (EDA)
Initial exploration was performed to understand:
- Column names and structure  
- Data types (categorical and numerical)  
- Presence of missing values  
- Overall shape of the dataset  

---

### 3. Dropping Unnecessary Columns
Irrelevant columns such as checking status, duration, purpose, and personal status were removed to reduce noise and improve data usability.

---

### 4. Column Name Standardization
Column names were cleaned and standardized by converting them to lowercase and replacing spaces with underscores for better readability and consistency.

---

### 5. Handling Duplicate Records
Duplicate rows were identified and removed to ensure data accuracy and prevent biased analysis.

---

### 6. Handling Missing Values
Missing values were checked across all columns and handled appropriately by removing affected rows to maintain data quality.

---

### 7. Cleaning and Transforming Categorical Data

#### Employment Column Transformation
The employment column contained categorical ranges representing employment duration.  
These values were first standardized (converted to lowercase and trimmed) and then mapped to numeric values based on approximate experience:

- `<1` → 0  
- `1<=x<4` → 2  
- `4<=x<7` → 5  
- `>=7` → 7  
- `unemployed` → 0  

This transformation makes the feature suitable for analysis and modeling.

---

#### Target Column Transformation
The class column (good/bad) was converted into binary numeric values:
- good → 1  
- bad → 0  

---

### 8. Data Type Conversion
Certain columns were originally in float format and were converted to integer values after rounding:

- age  
- existing_credits  
- num_dependents  
- residence_since  

This ensured consistency and improved data quality for further analysis.

---

### 9. Final Data Validation
Final checks were performed to ensure:
- No missing values remain  
- Correct data types are assigned  
- Data is clean and consistent  

---

### 10. Exporting Cleaned Data
The cleaned dataset was exported into:
- CSV format  
- Excel format  

This allows the data to be used for further analysis, reporting, or machine learning.

---

## ✅ Final Outcome
- Cleaned and structured dataset  
- Reduced number of columns  
- Standardized and consistent data  
- Ready for analysis and modeling  

---

## 📚 Key Learnings
- Performing structured data cleaning using Pandas  
- Handling missing values and duplicates  
- Standardizing and transforming categorical data  
- Converting data types for consistency  
- Preparing data for real-world analytics and machine learning  

---

## 💡 Conclusion
This project demonstrates a complete data cleaning workflow, starting from raw data exploration to producing a clean dataset ready for downstream applications such as analytics, visualization, and predictive modeling.
