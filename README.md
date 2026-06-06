# Data Cleaning Project – New York City Airbnb Open Data

## Objective
The objective of this project is to clean and preprocess the New York City Airbnb Open Data dataset to improve data quality and prepare it for analysis.

## Dataset
Dataset: AB_NYC_2019.csv

Total Records Before Cleaning: 48,895
Total Records After Cleaning: 45,923

## Data Cleaning Steps

### 1. Missing Value Handling
Missing values were found in:
- name
- host_name
- last_review
- reviews_per_month

Actions Taken:
- Filled missing names with "Unknown"
- Filled missing host names with "Unknown"
- Filled missing reviews_per_month with 0
- Converted last_review to datetime and filled missing values

### 2. Duplicate Removal
Checked for duplicate records and confirmed there were no duplicates.

### 3. Data Standardization
- Verified column data types
- Converted date fields to datetime format
- Standardized missing entries

### 4. Outlier Detection
Applied the IQR method on the price column:
- Identified extreme price values
- Removed outlier records

## Results
- Original Dataset Shape: (48895, 16)
- Cleaned Dataset Shape: (45923, 16)
- Missing Values Remaining: 0
- Duplicate Records Remaining: 0

## Key Insights
- Large numbers of missing values existed in review-related columns.
- Price distribution contained significant outliers.
- Data quality improved substantially after cleaning.
- The cleaned dataset is ready for visualization, analysis, and machine learning applications.

## Tools Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Outcome
Successfully transformed raw Airbnb listing data into a clean and reliable dataset suitable for data analysis and predictive modeling.
