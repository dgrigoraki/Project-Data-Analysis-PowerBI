# Power BI Energy Retail Customer & Billing Analytics

An end-to-end Power BI analytics project designed to clean raw transactional energy data, model relational data, and deliver key business insights on customer segmentation, billing performance, and overdue payment risks.

---

## Project Overview

This project addresses real-world data quality issues in energy retail management. Using **Power Query** and **DAX**, the dirty dataset was cleaned, transformed, and modeled with supporting dimension tables to build an interactive multi-page dashboard.

### Key Objectives:
* Perform data cleaning and transformation on raw transactional billing data.
* Build a relational Data Model connecting transactional facts with Customer and Tariff dimensions.
* Create custom DAX measures and calculated columns to answer core business questions.
* Identify high-risk customers with high energy consumption and overdue payments.

---

## Repository Structure

* **`Billing_Transactions_DIRTY.csv`** — Raw transactional dataset containing missing values, duplicates, and format inconsistencies.
* **`Customers.csv`** — Clean dimension table with customer segments, geographic data, and smart meter flags.
* **`Tariffs.csv`** — Clean dimension table with tariff types, pricing, and contract details.
* **`Project2.pbix`** — Interactive Power BI report file containing data model, DAX measures, and visuals.
* **`PowerBI_Energy_Retail_Project_Brief.pdf`** — Detailed walkthrough of data transformations and Power Query steps.
* **`PROJECT.docx`** — Executive summary answering analytical questions and providing business recommendations.

---

## Tools & Technologies Used
* **Power BI Desktop**
* **Power Query (M Code)** — Data Cleaning & Transformation
* **DAX (Data Analysis Expressions)** — Calculated Columns & Measures

---

## Key Data Cleaning Steps (Power Query)
* **Text Normalization:** Capitalized text fields, trimmed leading/trailing spaces, and removed invalid characters.
* **Deduplication:** Identified and removed duplicate transaction records.
* **Type Conversion:** Corrected date formatting issues (swapped month/day inconsistencies) and ensured proper numeric/currency data types.
* **Value Corrections:** Handled `NULL`/`N/A` values and converted negative numbers (invalid consumption/amounts) to positive values.

---

## Business Insights
* **Overdue Risk:** Identified specific customer segments with both high consumption and overdue payment statuses using custom DAX logical flags.
* **Smart Meters:** Analyzed complaint rates and billing patterns between smart meter and traditional meter users.
* **Tariff Performance:** Evaluated revenue and average invoice amounts across different tariff structures (e.g., Green Tariffs vs. Standard).
