# Viewership Analysis: Exploratory Data Analysis with Python

## 1. Project Overview

This project applies exploratory data analysis (EDA) using Python and pandas to examine viewership records. The exercise focuses on data cleaning, feature engineering, aggregation, and table joins to understand how viewing data can be prepared and summarised for further analysis.

The notebook was developed in Databricks as a practical exercise in data manipulation and exploratory analysis.

## 2. Project Objectives

- Inspect the dataset and assess its data quality.
- Identify and remove exact duplicate records.
- Extract date components and classify viewing-time values.
- Summarise viewing behaviour using grouping and aggregation.
- Understand inner, left, and outer joins using example tables.

## 3. Tools and Technologies

| Tool | Purpose |
|---|---|
| Python | Analytical programming |
| pandas | Data cleaning, feature engineering, aggregation, and joins |
| NumPy | Numerical computing |
| Databricks | Notebook development and execution |
| Excel | Source dataset |
| GitHub | Project documentation and version control |

## 4. Dataset Overview

The original dataset contains **118,534 rows and six columns**, covering customer identifiers, viewing time, platforms, play-event types, video titles, and date identifiers.

The notebook converts `DateID` into a datetime variable, `WatchDate`, to support date-based analysis.

## 5. Analysis Performed

### Data inspection and cleaning
- Examined the dataset's structure, column names, and data types.
- Checked for missing values and exact duplicate records.
- Removed duplicate rows using pandas.

### Feature engineering
- Extracted the day, month, and year from viewing dates.
- Classified records as weekday or weekend activity.
- Grouped recorded viewing times into Low, Med, and High categories using predefined thresholds.

### Aggregation
- Applied functions such as `count()`, `sum()`, `mean()`, `min()`, and `max()`.
- Used `groupby()` to summarise viewing records by platform, date-related categories, video title, and viewing-time category.
- Demonstrated how to count unique customers separately from total viewing records or viewing time.

### Table joins
- Used inner, left, and outer joins to explore how related tables can be combined using a common customer identifier.
- Demonstrated how unmatched customer and order records can be identified using example tables.

## 6. Key Findings

- **Data quality:** The initial inspection identified 9,873 exact duplicate rows, which were removed in the cleaned DataFrame.
- **Missing values:** The recorded checks reported no missing values in the inspected columns.
- **Customer coverage:** The original dataset contained 929 unique customer IDs.
- **Viewing categories:** Four platforms and four play-event types were identified.
- **Viewing-time range:** Recorded values ranged from 1 to 88,500; the measurement unit was not specified.
- **Analytical preparation:** Date-based features and viewing-time categories enabled grouped summaries of customer activity.

These findings are descriptive. Further investigation would be needed to establish the meaning of repeated records, validate viewing-time measurements, and draw conclusions about customer engagement.

## 7. Conclusion

The notebook demonstrates a foundational EDA workflow, from inspecting and cleaning raw data to engineering features, aggregating viewing records, and joining related tables. It provides practical experience with pandas and establishes a basis for more detailed analysis of viewing patterns and customer behaviour.

