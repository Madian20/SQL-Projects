# SQL Data Exploration Script  
**Language:** SQL Server (T-SQL)  
**Purpose:**  
This script performs a complete exploratory analysis of the database structure and the core business tables within the Gold Layer.  
It provides insights into customers, products, sales performance, and high-level KPIs.

---

## 🔍 What This Script Covers

### **1. Database Metadata**
- List all tables  
- List all columns  
Useful for understanding the schema and available objects.

### **2. Customer Insights**
- Countries of customers  
- Youngest & oldest customer  
- Customer distribution by country & gender  
- Total customers & active customers  

### **3. Product Insights**
- Categories, subcategories, product names  
- Total products  
- Average cost per category  

### **4. Sales Insights**
- First and last order dates  
- Range of years covered  
- Total revenue  
- Total quantity sold  
- Average selling price  
- Total orders  

### **5. Revenue Analysis**
- Revenue by category  
- Revenue by customer  
- Quantity distribution across countries  
- Top 5 products by revenue  
- Worst 5 products by revenue  

---

## 📦 Dataset Used
This script uses the following tables from the **Gold Layer**:

### **gold.dim_customers**
Customer demographic information.

### **gold.dim_products**
Product details and categorization.

### **gold.fact_sales**
Transactional sales data (core fact table).

---

## ✅ Output
Running this script gives you:
- Full understanding of data structure  
- Business KPIs  
- Customer & product segmentation  
- Revenue breakdowns  
- Identification of top & poor performing products  

