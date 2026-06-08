# Sales & Revenue Analysis Dashboard

## 📌 Problem Statement
Businesses generate large volumes of sales data but often struggle to identify revenue trends, profitable regions, top-performing products, and customer segments. This dashboard transforms raw sales data into actionable business insights.

---

## 🎯 Objective

- Analyze sales and profit performance
- Identify top-performing products and categories
- Track regional performance
- Monitor sales trends over time
- Support data-driven decision-making

---

## 📂 Dataset

**Dataset:** Superstore Sales Dataset

### Key Fields
- Order ID
- Order Date
- Customer ID
- Segment
- Category
- Sub-Category
- Region
- State
- Sales
- Profit
- Quantity

---

## ❓ Business Questions Solved

1. What is the total sales generated?
2. What is the total profit generated?
3. Which category contributes the highest revenue?
4. Which region generates the highest profit?
5. Which customer segment contributes the most sales?
6. What are the monthly sales trends?
7. Which products generate the highest revenue?
8. Which states contribute the highest sales?

---

## 📊 KPIs

- Total Sales
- Total Profit
- Total Orders
- Total Customers
- Profit Margin %

---

## 🛠 Power Query Transformations

- Removed null values
- Removed duplicate records
- Corrected data types
- Renamed columns
- Cleaned inconsistent values

---

## 🧮 DAX Measures

```DAX
Total Sales = SUM(Orders[Sales])

Total Profit = SUM(Orders[Profit])

Total Orders = DISTINCTCOUNT(Orders[Order ID])

Total Customers = DISTINCTCOUNT(Orders[Customer ID])

Profit Margin % =
DIVIDE([Total Profit],[Total Sales])*100
