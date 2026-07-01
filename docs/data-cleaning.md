# Data Cleaning

The data cleaning process is crucial for ensuring accuracy in the solar power generation analysis.

## Steps Taken:
1. **Handling Missing Values:** Null values were identified and dropped using dropna().
2. **Removing Duplicates:** Duplicate rows were eliminated to prevent skewed results.
3. **Negative Value Filtering:** Negative power generation values (impossible physics) were removed.
4. **Outlier Detection:** The IQR method was used on generated_power_kw to filter anomalies.
5. **Feature Selection:** Filtered the dataframe down to essential features.
