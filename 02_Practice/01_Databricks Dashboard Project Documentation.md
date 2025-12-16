# Databricks Dashboard Project Documentation

Author: Rishabh Bahuguna
Date: 16 December 2025

## 1. Project Overview

This project demonstrates the development of analytical dashboards using Databricks SQL and Spark-based queries. The objective was to transform structured datasets into interactive dashboards that support exploratory analysis and high-level reporting.

Two dashboards were developed:
- Transaction Dashboard based on retail sales data
- US Emissions Breakdown Dashboard based on public emissions data

The project focuses on data querying, metric definition, and dashboard design using native Databricks capabilities.

---

## 2. Scope of Work

The following activities were performed as part of this project:

- Queried structured datasets using Databricks SQL
- Performed aggregations and metric calculations within SQL queries
- Designed multiple datasets to support different dashboard views
- Built interactive dashboards using Databricks SQL Dashboards
- Implemented visualizations including bar charts, line charts, pie charts, scatter plots, and maps
- Added dashboard-level filters and descriptive annotations

---

## 3. Data Sources

### Transaction Dashboard

- **Dataset**: `samples.bakehouse.sales_transactions`
- **Source Type**: Databricks sample dataset
- **Data Type**: Structured transactional data
- **Key Fields**: product, quantity, totalPrice, paymentMethod, dateTime

### Emissions Dashboard

- **Dataset**: `emissions.default.emissions_data`
- **Source Type**: Public emissions dataset (EPA, 2023)
- **Data Type**: Structured geographic and emissions data
- **Key Fields**: county_state_name, state_abbr, population, GHG emissions mtons CO2e, latitude, longitude

---

## 4. Data Preparation and Transformations

Data preparation was handled directly within Databricks SQL queries.

Key transformation steps included:

- Casting string-based numeric fields into numeric data types
- Removing formatting characters such as commas before calculations
- Aggregating transactional data by product, date, and payment method
- Calculating per-capita emissions metrics using population data
- Creating summarized datasets for top states and counties by emissions

These transformations ensured the datasets were analysis-ready and performant for dashboard use.

---



## 5. Dashboard Design and Features

### Transaction Dashboard

- Bar chart showing total sales value by product
- Line chart displaying quantity sold over time
- Pie chart illustrating payment method distribution
- Global quantity filter using a range slider
- Descriptive text elements to provide context

### US Emissions Breakdown Dashboard

- Geographic map showing emissions locations across the continental US
- Scatter plot comparing emissions per person against population
- Pie chart highlighting the top 10 emitting states
- Bar chart ranking counties by total emissions
- Dashboard annotations describing data source and insights

The dashboards were designed to balance high-level summaries with the ability to explore underlying trends.

---

## 6. Tools and Technologies

- Databricks
- Databricks SQL
- Apache Spark
- Spark SQL
- Delta tables
- Databricks SQL Dashboards

---

## 7. Validation and Quality Checks

The following validation steps were performed:

- Verified aggregate results against raw dataset values
- Checked numeric conversions for accuracy
- Ensured consistent metric definitions across visualizations
- Reviewed dashboard outputs for logical consistency and clarity

---

End of Documentation




