# 🚀 MTA Bus Ridership Analytics Platform (Snowflake + Power BI)

## 📌 Overview
This project builds an end-to-end data analytics platform for MTA Bus ridership data using Snowflake and Power BI. It ingests raw transit data, transforms it into structured layers (RAW → STG → MART), and produces analytics-ready datasets used for reporting and decision-making.

---

## ❗ Business Problem
MTA operates hundreds of bus routes across NYC, generating large volumes of ridership data. However, identifying trends such as peak-demand periods, high-performing routes, and payment adoption (OMNY vs. MetroCard) requires structured data pipelines and consistent data modeling.

---

## 💡 Solution
Designed and implemented a scalable data pipeline in Snowflake:

- Ingest raw CSV data into staging tables
- Clean and standardize data for consistency
- Transform data into analytics-ready fact tables
- Deliver insights through Power BI dashboards

---

## 🧰 Tech Stack

- **Snowflake** – Data warehouse
- **SQL** – Data transformation and modeling
- **Power BI** – Data visualization and dashboards
- **Python** *(optional)* – Data handling / automation

---

## 🏗️ Data Architecture

- **RAW**: Ingested source data (no transformations)
- **STG**: Cleaned, typed, standardized data
- **MART**: Aggregated, business-ready datasets

---

## 📊 Key Insights

- Peak ridership occurs during weekday rush hours
- Certain routes consistently drive higher demand
- OMNY adoption is increasing relative to MetroCard
- Weekend ridership patterns differ significantly from weekdays

---

## 📈 Dashboard Features

Power BI dashboards provide:

- **Executive Overview** – Total ridership, trends, KPIs  
- **Route Analysis** – Top-performing routes  
- **Time Analysis** – Hourly and daily patterns  
- **Payment Analysis** – OMNY vs MetroCard usage  

*(See `/powerbi/dashboard.pbix` for full report)*

---

## ⚙️ Data Pipeline

1. Load CSV data into Snowflake (RAW layer)
2. Transform and clean data (STG layer)
3. Create aggregated tables (MART layer)
4. Connect Power BI to MART for reporting

---

## 🚀 Future Improvements

- Implement incremental data loading  
- Add anomaly detection for ridership spikes  
- Automate pipeline scheduling  
- Expand dataset coverage  

---


## 🧠 Key Takeaways

- Built an end-to-end data pipeline using Snowflake  
- Applied data modeling best practices (layered architecture)  
- Transformed raw data into business insights  
- Delivered analytics through Power BI dashboards  

---

## 📬 Contact

Daniel Souza  
Data Analyst | Power BI | Python | Snowflake  
![Snowflake](https://img.shields.io/badge/Snowflake-Data%20Warehouse-blue)
![Power BI](https://img.shields.io/badge/PowerBI-Dashboard-yellow)
![SQL](https://img.shields.io/badge/SQL-Data%20Modeling-lightgrey)

## 📂 Project Structure

```text
mta-bus-ridership-analytics/
├── README.md
├── sql/
│   ├── raw_tables.sql
│   ├── staging.sql
│   └── mart.sql
├── data/
│   └── sample.csv
├── powerbi/
│   └── dashboard.pbix
└── notebooks/
    └── pipeline.ipynb
