# E-Commerce Big Data Analytics Pipeline

A robust data engineering workflow designed to handle and analyze over **67 million rows** of e-commerce behavior data. This project demonstrates the transition from raw, unoptimized logs to structured PostgreSQL storage and business visualizations.

## Project Overview
The primary goal of this project was to engineer a scalable solution for processing massive e-commerce datasets. By leveraging **Apache Spark**, the pipeline addresses common "big data" challenges such as schema inconsistencies, massive null counts, and data redundancy.

## Tech Stack
* **Engine:** Apache Spark (PySpark)
* **Storage:** PostgreSQL
* **Analysis:** Pandas, SQL
* **Visualization:** Matplotlib, Seaborn

## Key Features & Workflow

### 1. Data Cleaning & Optimization
* **Scale:** Successfully processed 67M+ records of raw e-commerce event logs.
* **Integrity:** Implemented programmatic logic to handle significant null values, remove duplicates, and standardize schema inconsistencies.
* **Schema Enforcement:** Defined strict data types for event timestamps and price values to optimize memory usage and ensure data reliability.

### 2. Transformation & Storage
* **Aggregations:** Built complex Spark transformations to calculate daily traffic (Visits/Visitors), total revenue, and daily conversion rates.
* **Persistence:** Optimized the cleaned dataset and persisted it into a **PostgreSQL** database, creating a reliable foundation for downstream BI tools.

### 3. Analytics & Visualization
* **Data Bridge:** Converted specific Spark aggregation outputs to Pandas to enable localized, high-performance visualization.

---

## Insights & Visualizations

### Daily Traffic Trends
This chart illustrates the daily volume of sessions. Note the significant spike during the mid-month promotional events (Black Friday period).

![Daily Visits](./daily_visits_combined.png)

### Conversion Rate Performance
By analyzing the ratio of purchases to visits, we can identify "high-quality" traffic days. The data reveals that the mid-month surge was accompanied by a nearly triple increase in conversion efficiency.

![Conversion Rates](./conversion_rate_plot.png)

### Weekly Distribution (Outlier Analysis)
The box plots highlight the variance in traffic across different days of the week, identifying Sunday and Friday as the highest-performing periods for this dataset.

![Traffic Boxplot](./visits_by_day_boxplot.png)

---
