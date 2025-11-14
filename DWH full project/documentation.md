# Data Warehouse ETL (Bronze → Silver) – SQL Server

This project builds a simple Data Warehouse structure using **Microsoft SQL Server (T-SQL)** and implements a two-layer ETL pipeline: **Bronze** (raw data) and **Silver** (cleaned & standardized data).

## 📌 What the project does
- Creates the `DataWarehouse` database (if not exists)
- Builds **Bronze / Silver / Gold** schemas
- Creates all source tables in the Bronze layer
- Loads raw CSV files into Bronze using `BULK INSERT`
- Cleans, transforms, and standardizes the data into the Silver layer  
- Includes two ETL stored procedures:
  - `bronze.load_bronze` → Loads all raw CSVs  
  - `silver.load_silver` → Cleans & transforms Bronze data

## 📁 Layers Overview
### 🟫 Bronze Layer  
Raw CRM & ERP data loaded directly from CSVs (no cleaning, no transformations).

### ⚪ Silver Layer  
Cleaned, standardized, deduplicated, and type-corrected data.

## ▶️ How to Execute the ETL
After running the script and creating everything, execute the ETL with:

```sql
EXEC bronze.load_bronze;
EXEC silver.load_silver;
```

## 🎯 Goal
Build a clean and reusable ETL pipeline demonstrating:
- Data warehousing fundamentals  
- ELT/ETL structuring (Bronze → Silver)
- Practical SQL Server procedures  
- Realistic data cleaning rules (gender, marital status, deduplication…)

