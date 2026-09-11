# 🍽️ Restaurant Chain BI Dashboard

An interactive 3-page Power BI dashboard designed to analyze the performance of a 10-outlet restaurant chain operating across 5 major Indian cities.

The dashboard provides insights into revenue, profitability, customer ratings, outlet and item performance, and inventory wastage.

## 📊 Dashboard Preview

### 1. Executive Overview

Provides a high-level view of restaurant performance through key business KPIs, revenue trends, city-wise performance, service models, and outlet rankings.

![Executive Overview](Dashboard%20Screenshots/Output%20dashboard%201.jpeg)

### 2. Outlet & Item Performance

Analyzes outlet-level performance, customer ratings, day-wise revenue patterns, and item-level revenue and profitability.

![Outlet & Item Performance](Dashboard%20Screenshots/Output%20dashboard%202.jpeg)

### 3. Wastage & Inventory Monitor

Monitors inventory efficiency, wastage percentage, outlet-level wastage, stock health, and wastage cost against the target.

![Wastage & Inventory Monitor](Dashboard%20Screenshots/Output%20dashboard%203.jpeg)

---

## 🎯 Project Overview

The dashboard analyzes one year of restaurant data from **January 2025 to December 2025**, covering:

- 10 restaurant outlets
- 5 cities
- 7 menu items
- Revenue and food costs
- Customer ratings
- Service models
- Inventory and wastage data

The restaurant chain generated approximately **₹12M in annual revenue** with a **57.82% gross margin**.

---

## 📌 Key KPIs

| KPI | Value |
|---|---:|
| Total Revenue | ₹12.0M |
| Gross Margin | 57.82% |
| Gross Margin Value | ₹6.71M |
| Food Cost | 42.18% |
| Wastage | 6.97% |

---

## 📈 Dashboard Pages

### Executive Overview
- Total Revenue
- Gross Margin %
- Food Cost %
- Wastage %
- Revenue by City
- Revenue by Service Model
- Revenue Trend
- Revenue by Outlet
- Month-over-Month Growth

### Outlet & Item Performance
- Outlet-wise Revenue
- Average Customer Rating
- Gross Margin
- Food Cost %
- Day-of-week Revenue Heatmap
- Revenue vs Gross Margin by Item
- Revenue by Menu Item
- Revenue by Rating Band

### Wastage & Inventory Monitor
- Opening vs Closing Stock
- Wastage %
- Wastage by Outlet
- Item-level Wastage
- Stock Health Alerts
- Outlets with Inventory Issues
- Wastage Cost vs Target

---

## 🧠 Data Model

The project uses a **Star Schema** consisting of:

**Fact Table**
- Transactions

**Dimension Tables**
- Outlet
- Item
- Date
- Service Model

Power Query was used for data preparation and transformation before loading the data into the Power BI model.

---

## 📐 Key DAX Measures

### Total Revenue

```DAX
Total Revenue =
SUM(Transactions[Revenue])
