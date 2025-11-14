# Sales & Customer Analysis Documentation

This SQL analysis focuses on **sales performance over time**, **product performance**, **category contributions**, **product cost segmentation**, and **customer behavior**.  

## Data Sources
- **gold.fact_sales**: Contains all sales transactions.
- **gold.dim_customers**: Customer details including birthdate, gender, and country.
- **gold.dim_products**: Product details including category, subcategory, cost, and price.

## Analysis Components

1. **Sales Performance Over Time**
   - Monthly total sales, total customers, and total quantity sold.
   - Running total of sales and moving average price over time using window functions.

2. **Yearly Product Performance**
   - Compare each product's sales to its average sales and previous year’s sales.
   - Categorize performance as Above Average, Below Average, Increase, Decrease, or No Change.

3. **Category Contribution**
   - Calculate total sales per category.
   - Determine each category's contribution to overall sales (%).

4. **Product Cost Segmentation**
   - Segment products into cost ranges:
     - Below $100, $100-$500, $500-$1000, Above $1000
   - Count products per cost segment.

5. **Customer Segmentation**
   - Segment customers by spending behavior:
     - **VIP**: 12+ months history, spending > $5000
     - **Regular**: 12+ months history, spending ≤ $5000
     - **New**: < 12 months history
   - Count customers per segment.

6. **Customer Report View**
   - Consolidates all customer metrics at an individual level.
   - Includes total orders, total sales, quantity, products purchased, last order date, recency, average order value, and average monthly spend.
   - Segments customers by **age group** and **spending behavior**.
   - Available as the view: **`gold.customer_report`**

## Purpose
Provide a comprehensive overview of **sales trends, product and category performance, and customer behavior**, enabling informed decisions for marketing, sales strategy, and inventory planning.
