# 🐄 End-to-End Data Analytics & Business Case Study: Desi Dairy Farm (2019–2025)

## 📌 Project Overview
This repository presents a comprehensive, end-to-end data engineering and business analytics case study based on **7 years of authentic financial and operational ledgers** from *Desi Farm (SMC-Private) Limited*. 

Rather than relying on sanitized or simulated datasets, this project dives deep into a real-world agricultural business to uncover why a farm with millions in livestock assets struggled with cash flow, ultimately providing a data-driven root cause analysis backed by dairy industry standards.

The project is structured into two core phases:
1. **Data Engineering (ETL Pipeline):** Extracting, cleaning, and transforming raw, unstructured, multilingual data (English, Roman Urdu, Urdu script) from 13 disparate Excel sheets into analysis-ready datasets.
2. **Business Analytics & Case Study (EDA):** Differentiating operational cash flows from capital gains, assessing diet efficiency, and conducting a rigorous root cause analysis using FAO and NRC dairy management benchmarks.

---

## 🗂️ Repository Structure
- `data-cleaning-etl-desi-dairy-farm.ipynb`: The ETL pipeline script detailing the programmatic extraction and structuring of messy Excel ledgers.
- `desi-farm-case-study-exploratory-data-analysis.ipynb`: The master exploratory data analysis (EDA) notebook featuring time-series charts, dual-axis efficiency ratios, scatter regressions, and business conclusions.
- `Desi_Farm_Expenses.csv`: The cleaned, analysis-ready dataset for operational expenses.
- `Desi_Farm_Income.csv`: The cleaned, analysis-ready dataset for milk and operational revenues.

---

## 🚀 Phase 1: The ETL Pipeline (Data Engineering)
The raw source data consisted of 13 separate Excel files featuring irregular headers, floating charts, and unstructured text logs. The ETL script programmatically resolves these hurdles using **Python (Pandas)**:
* **Extraction & Structuring:** Automated ingestion across all 13 files, separating monthly income logs from daily/regular expense logs into clean, normalized DataFrames.
* **Text Standardization:** Handled multilingual free-text description logs containing local vendor names, worker salaries, and feed descriptions.
* **Datetime Parsing:** Converted irregular date strings into standardized datetime objects to enable smooth time-series aggregation.

---

## 📊 Phase 2: Business Case Study & Analytics
The analytical notebook answers critical business and financial questions across a 77-month lifecycle (July 2019 to October 2025):

### 1. The Cash Flow Illusion (Bulk Purchasing)
Identified how seasonal bulk purchasing of feed and fodder (e.g., silage and wheat straw during harvest months) heavily skews monthly cash flow negatively, which in turn subsidizes and creates apparent profitability in subsequent months.

### 2. The True Cost of Farming (Diet vs. Everything Else)
Demonstrated that separating Feed and Fodder dilutes their real impact. Grouping them into a single **"Diet"** category revealed that **68.2% of all operational expenses** are consumed exclusively by animal nutrition.

### 3. Comprehensive 77-Month Executive Audit
Calculated the true enterprise net worth by combining operational cash flows, livestock capital trading profits, and active on-farm inventory (**5.0 Million PKR** standing livestock assets), yielding an **Ultimate Grand Net Profit of 1.5 Million PKR** over 77 months at a 2.58% profit margin.

### 4. Operational Efficiency (Milk-to-Feed Ratio)
* Evaluated month-by-month efficiency by tracking Diet Cost as a percentage of Milk Income (skipping December 2019 outliers).
* Revealed an alarming average of **83.2%** of milk revenue going directly to feed costs—well above the healthy agricultural threshold.

### 5. Root Cause Analysis & Industry Citations
* **The "Procurement to Production" Death Spiral:** Proved via scatter regression analysis that month-to-month erratic purchasing and lack of an on-site **Total Mixed Ration (TMR)** caused severe dietary instability and rumen stress, suppressing milk yields.
* **Industry Benchmarks:** Validated findings using *FAO Dairy Production Guidelines* (recommending a 60%–70% diet cost limit) and *NRC Nutrient Requirements of Dairy Cattle* to demonstrate the biological and financial impact of inconsistent nutrition.

---

## 🛠️ Tools & Technologies
* **Language:** Python 3
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
* **Environment:** Kaggle Notebooks & GitHub Version Control
* **Data Source:** Authentic operational ledgers of Desi Farm (2019–2025)

---
*Authored by Imran Iqbal (بابا جی) — Professional Data Analyst & Online Mathematics Tutor.*
