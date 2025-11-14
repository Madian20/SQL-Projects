# 📊 Sales & Customer Analysis Documentation

This SQL analysis provides a **vivid overview of sales trends, product performance, and customer behavior**.  

---

## 🗂 Data Sources
- **gold.fact_sales** – All sales transactions 💰  
- **gold.dim_customers** – Customer details (birthdate, gender, country) 👥  
- **gold.dim_products** – Product details (category, subcategory, cost, price) 📦  

---

## 🔍 Analysis Components

### 1️⃣ Sales Performance Over Time
- Monthly total sales, total customers, and total quantity sold 📅  
- Running total of sales & moving average price over time using window functions 📈  

### 2️⃣ Yearly Product Performance
- Compare each product's sales to its **average** and **previous year** sales  
- Categorized as:  
  - ✅ Above Average  
  - ❌ Below Average  
  - 🔼 Increase  
  - 🔽 Decrease  
  - ➖ No Change  

### 3️⃣ Category Contribution
- Total sales per category 🏷  
- Contribution % of each category to overall sales 📊  

### 4️⃣ Product Cost Segmentation
- Products segmented by cost:  
  - 💲 Below $100  
  - 💲 $100 - $500  
  - 💲 $500 - $1000  
  - 💲 Above $1000  
- Count of products per cost segment 🔢  

### 5️⃣ Customer Segmentation
- Customers segmented by spending behavior:  
  - 👑 VIP: ≥12 months, spending > $5000  
  - 🏅 Regular: ≥12 months, spending ≤ $5000  
  - 🌱 New: <12 months  
- Count of customers per segment 📋  

### 6️⃣ Customer Report View
- Consolidates **all key metrics at the individual level**:  
  - Total orders, total sales, quantity, products purchased  
  - Last order date & recency  
  - Average order value & monthly spend 💵  
- Segmented by **age group** and **spending behavior**  
- Available as **`gold.customer_report`** 👁  

---

## 🎯 Purpose
Provide a **comprehensive, actionable view** of:  
- Sales trends over time ⏳  
- Product & category performance 📦  
- Customer behavior & segmentation 👥  

Enables **data-driven decisions** for marketing, sales strategy, and inventory planning ✅

