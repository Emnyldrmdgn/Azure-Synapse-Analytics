# Azure-Synapse-Analytics
Azure Synapse Analytics provides a single, consolidated data analytics platform for end-to end data analytics. In this exercise, you'll explore various ways to ingest and explore data. This exercise is designed as a high-level overview of the various core capabilities of Azure Synapse Analytics.

# Azure Synapse Analytics - Data Processing and Analysis Project

This project demonstrates how to use Azure Synapse Analytics for ingesting data into a data lake, querying with SQL, analyzing with Spark, and finally querying a data warehouse using a dedicated SQL pool.

## 🚀 Steps

### 1. Ingest Data
- The `products.csv` file was uploaded to Azure Data Lake.
- It was copied into the `files/product_data/` folder.
- File contents were previewed in Synapse Studio.

### 2. Query Data Using Serverless SQL Pool
- SQL queries were executed on `products.csv` using `OPENROWSET`.
- `HEADER_ROW = TRUE` was added to properly read column names.
- Data was grouped by category and visualized in a chart.
- The SQL script was saved as `Count Products by Category`.

### 3. Analyze Data with Spark Pool (PySpark)
- The CSV file was loaded into a Spark DataFrame using PySpark.
- `header=True` was set to enable proper column naming.
- Data was grouped by category and visualized in a chart.
- The notebook was named `Explore products` and published.

### 4. Query a Data Warehouse Using Dedicated SQL Pool
- The dedicated SQL pool `sqlxxxxxxx` was resumed.
- A query was run on the `FactInternetSales`, `DimDate`, and `DimProduct` tables:
  - The total quantity of products sold was grouped by year, month, and product.
- The SQL script was saved as `Aggregate product sales`.

### 5. Clean Up Azure Resources
- The Spark and SQL pools were paused.
- The `dp203-xxxxxxx` resource group was deleted to avoid extra costs.

## 📁 Created Files and Scripts
- `products.csv`
- `Count Products by Category` (SQL Script)
- `Explore products` (Spark Notebook)
- `Aggregate product sales` (SQL Script)

---

## 📌 Requirements
- Azure Subscription
- Azure Synapse Workspace
- Azure Data Lake Storage
- Access to Synapse Studio

---

## 🎯 Goal
To learn and implement an end-to-end data analytics workflow using Azure Synapse, combining data lake, data warehouse, and analytics tools in one unified platform.

