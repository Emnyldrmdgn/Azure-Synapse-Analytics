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

## ScreenShots
![lab12](https://github.com/user-attachments/assets/66a1cdb0-2c92-4ce2-8dec-efeb8befa586)
![lab13](https://github.com/user-attachments/assets/ee655934-4271-4f2c-8515-8e3606ab926f)
![lab14](https://github.com/user-attachments/assets/6e549d2d-08c6-42ac-a120-48fdcbc3764b)
![lab15](https://github.com/user-attachments/assets/3e9919d5-3ac7-4296-8f7c-c20603178f98)
![lab16](https://github.com/user-attachments/assets/c3fc341e-4fd7-4db4-8cef-a76724350925)
![lab17wspace](https://github.com/user-attachments/assets/7d43e64e-d827-49f9-86b4-189ec509623d)
![lab18manage](https://github.com/user-attachments/assets/b7552d7d-1685-4bbc-9ff4-ea12f21160f8)
![lab19copydata](https://github.com/user-attachments/assets/0b603bae-f300-4026-a718-c5e400b67b80)
![lab120data](https://github.com/user-attachments/assets/9a176ff9-3266-48d5-9b94-f36d08e7da38)
![lab120data2](https://github.com/user-attachments/assets/d22f701b-9b4a-4115-a117-c6e49816755f)
![lab120data3](https://github.com/user-attachments/assets/f5d3206a-0721-41b4-a2da-8c2bd1589c83)




