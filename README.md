# 📊 Smart Inventory Intelligence System
### Stock-Out Risk & Demand Analytics Dashboard

An interactive data analytics and inventory monitoring system designed to help businesses understand inventory levels, identify stock-out risks, analyze demand, and make better reorder decisions.

---

## 📌 Project Overview

Inventory management is an important part of retail and supply-chain operations. Maintaining too much inventory can increase holding costs, while insufficient inventory can lead to stock-outs and lost sales.

The **Smart Inventory Intelligence System** analyzes historical inventory, sales, ordering, pricing, and demand forecast data to identify stock-out risks and provide useful inventory insights.

The project includes an interactive web-based dashboard that allows users to filter and analyze inventory data by:

- Store
- Product Category
- Region
- Date

The dashboard presents important KPIs, charts, risk analysis, and reorder recommendations in an easy-to-understand format.

---

## 🎯 Problem Statement

Businesses often have large amounts of inventory and sales data, making it difficult to identify products or stores that are at risk of stock-outs.

Traditional inventory monitoring may require manually checking large datasets, which can be time-consuming and may delay decision-making.

This project aims to develop a data-driven inventory analytics system that can:

- Monitor inventory levels
- Analyze sales and demand
- Identify stock-out risks
- Compare demand forecasts with actual sales
- Provide reorder recommendations
- Present insights through an interactive dashboard

---

## 💡 Proposed Solution

The proposed system processes inventory and sales data using Python and Pandas and performs analytical calculations to determine inventory conditions and stock-out risks.

A Flask backend provides APIs for retrieving analytical results, while the frontend uses HTML, CSS, JavaScript, and Chart.js to display the results through interactive visualizations.

The system converts raw inventory data into meaningful insights that can support better inventory management decisions.

---

## ✨ Key Features

### 📊 Interactive Dashboard

The dashboard provides a centralized view of important inventory and sales information.
## 🖥️ Dashboard Preview

### Dashboard Overview

![Dashboard Overview](screenshots/dashboard.png)

### Analytics & Visualizations

![Analytics Charts]("C:\Users\KRUSHITHA\OneDrive\Desktop\DAV_LAB\Screenshorts\charts_1.png"")
![Analytics Charts](screenshots/charts_2.png")

### Risk & Reorder Watchlist

![Risk and Reorder Watchlist](screenshots/risk-watchlist-1.png)
![Risk and Reorder Watchlist](screenshots/risk-watchlist-2.png)
![Risk and Reorder Watchlist](screenshots/risk-watchlist-3.png)
![Risk and Reorder Watchlist](screenshots/risk-watchlist-4.png)


### 🔍 Dynamic Filters

Users can filter the dashboard based on:

- Store
- Category
- Region
- Date range

### 📈 KPI Monitoring

The dashboard displays important Key Performance Indicators such as:

- Total Inventory
- Total Units Sold
- Total Units Ordered
- Demand Forecast
- Stock-Out Risk
- Other relevant inventory metrics

### 📦 Inventory Analysis

The system analyzes current inventory levels across different:

- Stores
- Product categories
- Regions

### 📉 Demand Analysis

The dashboard compares:

- Demand Forecast
- Actual Units Sold
- Demand Difference

This helps identify differences between expected and actual demand.

### ⚠️ Stock-Out Risk Detection

Products are categorized based on their stock-out risk:

- 🟢 Low Risk
- 🟡 Medium Risk
- 🔴 High Risk

### 🔄 Reorder Recommendations

The system provides reorder recommendations based on inventory conditions and demand analysis.

### 🏪 Store-wise Analysis

Users can analyze:

- Store-wise inventory
- Store-wise sales
- Store-level stock conditions

### 📊 Interactive Visualizations

The dashboard includes visualizations such as:

- Units Sold by Category
- Current Inventory by Category
- Demand Forecast vs Units Sold
- Stock-Out Risk Distribution
- Store-wise Inventory
- Store-wise Sales
- Risk & Reorder Watchlist

---

## 🗂️ Dataset

The project uses a retail inventory dataset containing information related to stores, products, sales, inventory, orders, demand forecasts, and pricing.

### Main Dataset Attributes

| Column | Description |
|---|---|
| Date | Date of the recorded transaction |
| Store ID | Unique identifier for the store |
| Product ID | Unique identifier for the product |
| Category | Product category |
| Region | Store/market region |
| Inventory Level | Current inventory quantity |
| Units Sold | Number of units sold |
| Units Ordered | Number of units ordered |
| Demand Forecast | Forecasted demand |
| Price | Product price |
| Demand Difference | Difference between demand forecast and actual sales |
| Stock Coverage | Estimated inventory coverage |
| Stock-Out Risk | Risk level of stock-out |
| Reorder Recommendation | Suggested inventory action |

---

## 🧹 Data Preprocessing

The dataset was processed before performing analysis.

The preprocessing steps included:

1. Loading the raw dataset
2. Checking data types
3. Checking for missing values
4. Checking for duplicate records
5. Cleaning and preparing the dataset
6. Creating derived analytical features
7. Calculating demand difference
8. Calculating stock coverage
9. Determining stock-out risk
10. Generating reorder recommendations

The cleaned dataset was then used for analysis and visualization.

---

## 📐 Analytical Measures

### Demand Difference

Demand Difference helps compare forecasted demand with actual units sold.

```text
Demand Difference = Demand Forecast - Units Sold
