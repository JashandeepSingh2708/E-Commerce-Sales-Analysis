# E-Commerce-Sales-Analysis
 Power BI dashboard for E-Commerce Sales Analysis. Analyzes profit, orders, revenue, payment modes, and product categories across months, cities, and states. Offers business insights with dynamic filters and DAX-based KPIs like Average Order Value.


# 📊 E-Commerce Sales Analysis Dashboard (Power BI)

This Power BI project delivers a dynamic and interactive dashboard for analyzing e-commerce sales across key dimensions such as time, geography, category, and payment modes. The dashboard offers granular insights with state and quarterly filters, helping uncover patterns in profitability, quantity, and customer behavior.

---

## 📁 Dataset Overview

### 🔹 Orders Table:
- Order ID
- Order Date
- Customer Name
- State
- City

### 🔹 Details Table:
- Order ID
- Amount
- Profit
- Quantity
- Category
- Sub-Category
- Payment Mode

---

## 🧮 DAX Measure Used

```dax
Average Order Value =  
DIVIDE(
    SUM('Details (2)'[Amount]),
    DISTINCTCOUNT('Orders (2)'[Order ID])
)
---
## 🔍 Key Insights

- 💰 **Profit Peaks**: December tops with ₹10.3K profit, followed by January (₹9.7K) and February (₹8.5K)
- 📉 **Loss-Making Months**: May (-₹3.7K), June (-₹2.1K), and October (-₹1.4K) recorded negative profits
- 🖨️ **Top Sub-Categories by Profit**: Printers (₹8.6K), Bookcases (₹6.5K), Sarees (₹4.1K)
- 👚 **Most Sold Category**: Clothing leads in quantity (3.5K), well ahead of Electronics (1.2K) and Furniture (0.9K)
- 🏙️ **Top 3 Cities by Order Volume**: Indore (71), Mumbai (67), Chandigarh (30)
- 💳 **Popular Payment Methods**: COD dominates at 45.6%, followed by UPI (22.1%) and Debit Card (13.5%)

### 📦 Overall Metrics:
- **Total Revenue**: ₹438K  
- **Total Profit**: ₹37K  
- **Total Orders**: 500  
- **Average Order Value**: ₹876  

---

## 📌 Dashboard Features

- ✅ Filters: State-wise & Quarter-wise analysis
- 📆 Monthly profit tracking
- 📦 Product sub-category profitability
- 🛍️ Sales quantity by category
- 🏙️ City-wise order distribution
- 💳 Payment mode distribution (donut chart)
- 🌙 Dark-themed UI for better contrast and readability

---

## 🎯 Use Cases

- For job seekers to showcase Power BI & DAX skills
- For business stakeholders to derive actionable insights
- For data enthusiasts exploring real-world BI projects

---

## 🛠️ Tools & Technologies

- Microsoft Power BI
- DAX (Data Analysis Expressions)
- Data Modeling (Orders ↔ Details via Order ID)
