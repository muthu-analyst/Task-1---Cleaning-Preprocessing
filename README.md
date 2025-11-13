# Task-1---Cleaning-Preprocessing


## Project Description
This project focuses on cleaning and preprocessing a marketing dataset to prepare it for downstream analysis and modeling. The dataset contains various customer demographic and purchase-related features collected from marketing campaigns.

## What I Did

- **Data Inspection:** Examined the dataset for structure, missing values, duplicates, and data types.
- **Duplicates Removal:** Checked for and removed duplicate rows to avoid data redundancy.
- **Missing Value Handling:** Identified missing values mainly in the `income` column; missing income values were imputed with the median income.
- **Data Type Conversion:**
  - Converted date column (`dt_customer`) to datetime format and then formatted it to `dd-mm-yyyy` string format based on requirements.
  - Converted categorical fields like `education`, `marital_status`, and `country` to the category data type for optimized storage and processing.
- **Outlier Handling:** Detected and removed outliers in the `income` column by trimming values outside the 1st and 99th percentile range.
- **Column Name Standardization:** Trimmed whitespace from column names, converted them to lowercase, and replaced spaces with underscores for consistency.

## How to Run

1. Place the raw dataset (`marketing_data.csv`) in the project folder.
2. Run the data cleaning script (`clean_preprocess.py`) which applies all the above preprocessing steps and outputs a cleaned dataset as `marketing_data_cleaned.csv`.
