Task 1: Data Cleaning and Preprocessing

Overview
This repository contains the solution for **Task 1: Data Cleaning and Preprocessing**.  
The objective of this task was to clean and prepare a raw dataset for analysis by handling missing values, duplicates, inconsistent formats, and data types using **Python (Pandas)**.

Dataset Used:  
- `sales.csv` (contains sales data for multiple stores, including weekly sales, date, temperature, fuel price, CPI, unemployment, and holiday flags)  
- Dataset downloaded from Kaggle (or local dataset provided).
- 
Steps Performed

1. Loaded the dataset
   - Used `pandas.read_csv()` to load the CSV file.  
   - Checked the initial shape and first few rows of the dataset.

2. Checked for missing values and duplicates
   - Used `.isnull().sum()` to identify missing values.  
   - Used `.duplicated().sum()` to identify duplicate rows.

3. Handled missing values
   - Filled numeric columns with the median value using `fillna()`.  
   - Dropped any remaining nulls using `dropna()`.

4. Removed duplicate rows*
   - Used `drop_duplicates()` to remove duplicates if any existed.

5. Standardized text columns 
   - Converted all object (text) columns to lowercase and removed extra spaces.

6. Converted date column to datetime format
   - Converted the `Date` column from string to `datetime` using `pd.to_datetime()` for consistency.  
   - Ensures proper chronological sorting and date-based analysis.

7. Renamed columns
   - Converted column names to `snake_case` (lowercase, underscores instead of spaces).

8. Checked and fixed data types
   - Ensured numeric columns are correctly typed (`int` or `float`).  
   - Optional columns like `age` handled if present.

9. Saved the cleaned dataset 
   - The cleaned dataset is saved as `cleaned_dataset.csv` ready for analysis.

---

Cleaning Summary

| Step | Status |
|------|--------|
| Missing values handled | ✅ |
| Duplicate rows removed | ✅ |
| Text columns standardized | ✅ |
| Date column converted | ✅ |
| Column names cleaned | ✅ |
| Data types checked & corrected | ✅ |
| Cleaned dataset saved | ✅ |


