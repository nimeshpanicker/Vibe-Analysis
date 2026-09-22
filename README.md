# 📊 Vibe Analysis — E-commerce Business Performance Analysis

## 📌 Project Overview

Vibe Analysis is an end-to-end e-commerce data analytics project demonstrating a complete Data Analyst workflow:

**Raw Data → Data Profiling → Data Cleaning → Star Schema → Business Analysis → Interactive Dashboard**

The project analyzes sales, profit, customers, products, categories, regions, and monthly business performance.

The final analytical dataset contains:

- 25,000 unique orders
- 2,000 unique customers
- 100 products
- 731 unique dates
- January 2024 – December 2025

---

## 🎯 Business Questions

The analysis answers key business questions:

1. What are the top 10 products by revenue?
2. Which regions generate the highest profit?
3. What are the monthly revenue and profit trends?
4. Which products generate high revenue but low profit margins?

---

## 🛠️ Tools & Technologies

- SQL
- Excel
- Python-assisted data workflow
- HTML
- JavaScript
- Chart.js
- GitHub
- Data Cleaning
- Data Profiling
- Star Schema / Dimensional Modeling
- Business Intelligence

---

## 📂 Source Data

The project started with four raw datasets:

- Customers
- Orders
- Products
- Regions

The raw orders dataset contained 25,050 rows, while the customer dataset contained 2,010 rows. The product dataset contained 100 products and the region dataset contained 20 records.

---

## 🧹 Data Cleaning

The data-quality process identified:

- 50 exact duplicate order transactions
- 10 invalid order dates
- 60 missing customer IDs
- 35 missing product IDs
- 15 negative-quantity transactions
- 15 profit calculation mismatches
- 10 duplicate customer records
- Inconsistent product-category formatting

The cleaned customer dimension contains 2,000 unique customers.

Product categories were standardized, while potentially inconsistent category/sub-category combinations were flagged for review.

An `is_return` indicator was created for negative-quantity transactions.

---

## ⭐ Analytical Data Model

A star-schema approach was designed for the analysis.

### Fact Table

`Fact_Orders`

Contains:

- Sales amount
- Cost
- Profit
- Quantity
- Discount
- Transaction keys

### Dimension Tables

- `Dim_Customers`
- `Dim_Products`
- `Dim_Regions`
- `Dim_Date`

The date dimension contains:

- Date Key
- Date
- Day
- Month
- Month Name
- Quarter
- Year

---

## 📊 Key Business Results

### Overall Performance

| KPI | Result |
|---|---:|
| Total Revenue | ₹29.50M |
| Total Profit | ₹6.76M |
| Profit Margin | 22.9% |
| Unique Orders | 25,000 |
| Unique Customers | 2,000 |
| Return Transactions | 15 |

---

## 🌍 Regional Performance

North generated the highest total profit at approximately **₹1.72M**.

Central generated substantially lower revenue and profit than the other regions, while its profit margin remained broadly similar.

---

## 🛍️ Category Performance

**Home & Kitchen** generated the highest category revenue at approximately **₹6.76M**.

**Furniture** recorded the highest category profit margin at approximately **25.6%**.

---

## 🏆 Top Products by Revenue

The highest-revenue products included:

1. Kids Product 98
2. Tables Product 97
3. Storage Product 83
4. Appliances Product 99
5. Appliances Product 50
6. Cookware Product 59
7. Kids Product 80
8. Women Product 67
9. Chairs Product 12
10. Paper Product 94

---

## ⚠️ High Revenue but Low Profit Margin

Two products were identified as generating relatively high revenue but weak profitability:

| Product | Revenue | Profit | Margin |
|---|---:|---:|---:|
| Cookware Product 89 | ₹501K | ₹48K | 9.6% |
| Mobiles Product 66 | ₹417K | ₹50K | 12.1% |

These products can be investigated further for pricing, costs, discounts, and supplier-related factors.

---

## 📅 Monthly Performance

The analysis covers **24 months from January 2024 to December 2025**.

- Highest monthly revenue: **December 2025 — ₹1.33M**
- Highest monthly profit: **August 2025 — ₹303K**

The highest-revenue month was different from the highest-profit month, demonstrating why revenue should be analyzed together with profitability.

---

## 📈 Interactive Dashboard

The project includes an interactive HTML dashboard with:

- Total Revenue
- Total Profit
- Total Orders
- Unique Customers
- Monthly Revenue & Profit Trend
- Revenue by Category
- Profit by Region
- Top 10 Products by Revenue

### Filters

- Year
- Region
- Category

---

## 📄 Project Report

[View Vibe Analysis Project Report](reports/Vibe_Analysis_Ecommerce_Report.pdf)

---

## 🔄 Project Workflow

```text
Raw CSV Data
     ↓
Data Profiling
     ↓
Data Quality Assessment
     ↓
Data Cleaning
     ↓
Dimension & Fact Tables
     ↓
Star Schema
     ↓
Business Analysis
     ↓
Interactive HTML Dashboard
     ↓
Business Insights
