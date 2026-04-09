# 🛒 Online Retail Sales Dashboard — Power BI

Author : Blessed Mavhemwa

## Project Overview

This project analyzes an online retail dataset to uncover sales trends, customer behavior, and product performance. An interactive Power BI dashboard was built to visualize key business metrics, enabling data-driven decision-making across revenue, customer, and product dimensions.

---

## 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| **Python (Pandas)** | Data cleaning and preprocessing |
| **Power BI Desktop** | Dashboard design and data visualization |
| **DAX (Data Analysis Expressions)** | Creating calculated measures and KPIs |
| **Power Query** | Data transformation within Power BI |

---

## 📦 Dataset Description

- **Source:** Online Retail transactional dataset
- **Table Name:** `cleaned_online_retail`
- **Records:** ~500,000+ transactions
- **Time Period:** 2010 – 2011

### Columns

| Column | Description |
|--------|-------------|
| `InvoiceNo` | Unique invoice/order number |
| `StockCode` | Product stock code |
| `Description` | Product name/description |
| `Quantity` | Number of units purchased |
| `InvoiceDate` | Date and time of the transaction |
| `UnitPrice` | Price per unit (GBP) |
| `CustomerID` | Unique customer identifier |
| `Country` | Country where the customer is located |
| `Revenue` | Calculated column: Quantity × UnitPrice |

---

## 🧹 Data Cleaning

The following cleaning steps were applied to the raw dataset before loading into Power BI:

- **Removed null values** in `CustomerID` and `Description` columns
- **Removed cancelled orders** (invoices starting with `C`)
- **Filtered out negative quantities** and zero/negative unit prices
- **Created a `Revenue` column** by multiplying `Quantity` × `UnitPrice`
- **Standardized date formats** for the `InvoiceDate` column
- **Removed duplicate records** to ensure data integrity
- **Saved the cleaned dataset** as `cleaned_online_retail` for use in Power BI

---

## 📊 Dashboard Visualization

The dashboard is built on a single **Executive Summary** page with the following visuals:

### KPI Cards (Top Row)
- **Total Revenue** — 8.91M
- **Total Quantity** — 5M
- **Total Orders** — 19K
- **Average Order Value** — 480.87
- **Total Customers** — 4K

### Charts & Visuals

| Visual | Type | Description |
|--------|------|-------------|
| Revenue Trend by Month | Line Chart | Shows monthly revenue across the year |
| Top Products by Quantity | Bar Chart | Ranks top products by units sold |
| Revenue by Country | Bar Chart | Compares revenue across all countries |
| Revenue by CustomerID | Donut Chart | Breakdown of revenue contribution per customer |

### Slicers / Filters
- **Month** slicer — filter all visuals by month
- **Country** slicer — filter all visuals by country
- **Year** slicer — filter all visuals by year

---

## 💡 Key Insights

1. **Revenue peaks in Q4** — November and December show the highest monthly revenue, likely driven by seasonal holiday shopping.

2. **United Kingdom dominates sales** — The UK accounts for the vast majority of total revenue, far exceeding all other countries combined.

3. **Top products are gift/novelty items** — Products like *Paper Craft Little Birdie*, *Medium Ceramic Top*, and *World War 2 Gliders* consistently rank among the highest sellers by quantity.

4. **Small customer base drives high revenue** — With only ~4K unique customers generating 8.91M in revenue, the average order value is high (480.87), suggesting bulk or repeat purchasing behavior.

5. **International markets are underutilized** — Countries like Netherlands, EIRE, Germany, and France show promising revenue figures but remain significantly behind the UK, indicating growth opportunities.

6. **Consistent order volume** — 19K total orders across the period suggests a stable and loyal customer base with regular purchasing patterns.


## 📸 Dashboard Review
<img width="993" height="578" alt="Executive Summary" src="https://github.com/user-attachments/assets/256fb4a6-4f1c-4b65-913e-701561e9849c" />
