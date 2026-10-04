# Credit Card Fraud Detection Dashboard

## Overview
Analyzed 555,719 credit card transactions to identify patterns in fraudulent activity. Built a full relational data pipeline using SQL Server, Python, Excel, and Power BI, with dual dashboard versions and custom DAX measures for data modeling practice.

## Tools Used
- **Python (pandas)** — data cleaning and splitting a flat dataset into a relational schema (customers, merchants, transactions, date dimension)
- **SQL Server (SSMS)** — relational database with primary/foreign keys, and 6 custom SQL views for fraud analysis
- **Excel** — Power Query, PivotTables, and PivotCharts dashboard
- **Power BI** — star-schema data model with auto-detected relationships, custom DAX measures (CALCULATE, ALLEXCEPT, RANKX), and an interactive dashboard

## Key Findings
- Overall fraud rate: 0.39% (2,145 fraud cases out of 555,719 transactions)
- Fraud peaks sharply between 10–11 PM, nearly 5x the baseline rate
- Weekends show a higher fraud rate than weekdays
- Grocery (point-of-sale) is the merchant category with the highest fraud rate
- Among customer jobs with reliable sample sizes (100+ transactions), horticultural consultants had the highest fraud rate (5.6%)

## Files
- `fraud_detection_analysis.ipynb` — full Python data cleaning and SQL push pipeline
- `fraudTest_clean.xlsx` — original raw dataset
- `customers.csv`, `merchants.csv`, `transactions.csv`, `date_dim.csv` — cleaned, split relational tables
- `schema_setup.sql` — table keys and relationships
- `fraud_views.sql` — 6 SQL analysis views
- `fraud_dashboard.xlsx` — Excel dashboard
- `fraud_dashboard.pbix` — Power BI dashboard

## Dataset Source
[Kaggle: Credit Card Transactions Fraud Detection Dataset](https://www.kaggle.com/datasets/kartik2112/fraud-detection)

## Author
Meera — Data with Meera
