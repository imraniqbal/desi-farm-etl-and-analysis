# 🐄 End-to-End Data Analytics: Desi Dairy Farm (2019–2025)

## 📌 Project Overview
This repository contains an end-to-end data engineering and analytics portfolio project based on a 7-year real-world financial and operational ledger. The project is divided into two core phases: 
1. **ETL Pipeline:** Extracting and cleaning raw, unstructured, multilingual data from 13 messy Excel files.
2. **Case Study & Analytics:** Analyzing the cleaned data to extract business insights, operational costs, and profitability metrics.

## 🏢 Business Context & The Data
The dataset originates from the daily operational ledgers of **Desi Farm (SMC-Private) Limited**. As a continuous log spanning from 2019 to 2025, it captures authentic agricultural expenses, including feed, fodder, veterinary medicines, maintenance, and salaries. 

Unlike sanitized practice datasets, these are authentic logs. A unique challenge of this dataset is the `Description` column, which contains a natural, real-world mix of English, Roman Urdu, and standard Urdu script, alongside specific references to local vendors and farm workers.

## 🗂️ Repository Structure
This repository utilizes a flat, accessible structure containing two primary Python notebooks and the resulting datasets:

* `etl_pipeline.ipynb`: The Data Engineering notebook detailing the extraction and transformation of the raw Excel files.
* `case_study_analysis.ipynb`: The Data Analytics notebook containing exploratory data analysis (EDA), time-series forecasting, and visualizations.
* `Desi_Farm_Expenses.csv`: The cleaned, analysis-ready dataset for farm expenses.
* `Desi_Farm_Income.csv`: The cleaned, analysis-ready dataset for farm income.

## 🚀 Phase 1: The ETL Pipeline
The raw data consisted of 13 separate Excel files featuring unstructured layouts, floating charts, and irregular headers. The ETL script (`etl_pipeline.ipynb`) utilizes **Python (Pandas)** to programmatically resolve these challenges:
* **Extraction:** Bypassed irregular spreadsheet formatting and automated the extraction across all 13 files.
* **Structural Separation:** Successfully separated income (logged monthly) and expenses (logged daily/regularly) into two distinct DataFrames.
* **Transformation:** Standardized column names, dropped null artifacts, and converted string dates into standardized datetime objects.

## 📊 Phase 2: Case Study & Analytics (Upcoming)
The analytics phase (`case_study_analysis.ipynb`) will leverage the cleaned data to answer critical business questions, focusing on:
* **Cost Drivers:** Identifying the largest operational expenses (e.g., feed vs. electricity) and their seasonal variations.
* **Profitability Margins:** Merging the income and expense timelines to visualize net monthly margins.
* **Text Categorization:** Applying NLP techniques to extract structured insights from the multilingual, free-text description logs.

## 🛠️ Tools & Technologies
* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
* **Environment:** Kaggle Notebooks
* **Data Source:** [Dairy Farm Operations & Financial Ledger 2019–2025 (Kaggle)](https://www.kaggle.com/datasets/imran495/dairy-farm-operations-and-financial-ledger-20192025)
