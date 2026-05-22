# 🛒 Superstore Sales Dashboard — Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-185FA5?style=for-the-badge&logo=microsoft&logoColor=white)
![Power Query](https://img.shields.io/badge/Power%20Query-1D9E75?style=for-the-badge&logo=microsoft&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)

> An end-to-end interactive sales dashboard built on the Superstore dataset — covering data cleaning, DAX measures, and rich visual storytelling.

---

## 📌 Project Overview

This project demonstrates a complete **Business Intelligence workflow** using Microsoft Power BI:

- 🧹 Raw data cleaning in **Power Query**
- 📐 Custom KPI measures using **DAX**
- 📊 Interactive dashboard with **slicers, charts & KPI cards**
- 💡 Actionable business insights from **9,994 rows** of sales data

---

## 📊 Key KPIs

| Metric | Value |
|---|---|
| 💰 Total Sales | $2.29M |
| 📈 Total Profit | $286K |
| 📉 Profit Margin | 12.47% |
| 🛒 Total Orders | 9,994 |
| 📦 Quantity Sold | 38K |

---

## 🧹 Data Cleaning — Power Query

The raw dataset had several quality issues that were fixed in Power Query:

- ✅ Removed **null values** across key columns
- ✅ Fixed **date format** inconsistencies (dates stored as numbers/text)
- ✅ Identified and removed true **duplicate rows** (kept multiple products per Order ID intact)
- ✅ Trimmed and cleaned **text fields** for consistency
- ✅ Validated data integrity across all **9,994 rows**

---

## 📐 DAX Measures

```dax
-- Profit Margin %
Margin % = DIVIDE(SUM('Sample - Superstore'[Profit]), SUM('Sample - Superstore'[Sales])) * 100

-- Total Sales
Total Sales = SUM('Sample - Superstore'[Sales])

-- Total Profit
Total Profit = SUM('Sample - Superstore'[Profit])

-- Total Orders
Total Orders = DISTINCTCOUNT('Sample - Superstore'[Order ID])

-- Quantity Sold
Quantity Sold = SUM('Sample - Superstore'[Quantity])
```

---

## 📈 Dashboard Visuals

| # | Chart | Type | Insight |
|---|---|---|---|
| 1 | Sales & Profit by Year | Line Chart | Growth trend 2014–2017 |
| 2 | Sales by Sub-Category | Horizontal Bar | Best/worst product lines |
| 3 | Profit by Region | Donut Chart | Regional profit share |
| 4 | Top 5 Customers by Sales | Bar Chart | High value customers |
| 5 | Sales by Category | Treemap | Category revenue breakdown |
| 6 | Orders by Ship Mode | Treemap | Shipping preference |
| 7 | Category Summary | Table | Sales, Profit & Margin % |

### 🎛️ Slicers
- **Year** — 2014, 2015, 2016, 2017 (Tile style)
- **Region** — Central, East, South, West (Tile style)

---

## 💡 Key Business Insights

- 📌 **Technology** is the most profitable category at **17.4% margin**
- 📌 **Furniture** has a dangerously low margin of just **2.49%**
- 📌 **West region** leads profit contribution at **37.86%**
- 📌 **Sean Miller** is the top customer with **$25K** in sales
- 📌 **Standard Class** is the most preferred shipping mode
- 📌 Sales grew consistently from **$484K (2014) → $733K (2017)**

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Power BI Desktop** | Dashboard creation & visualization |
| **Power Query** | Data cleaning & transformation |
| **DAX** | Custom measures & calculations |
| **Microsoft Excel** | Source data format (.xlsx) |

---

## 🚀 How to Run This Project

1. Download the `.pbix` file from this repository
2. Open it in **Power BI Desktop** (free download from Microsoft)
3. The dataset is embedded — no additional setup needed
4. Use the **Year** and **Region** slicers to explore the dashboard interactively

---

## 📸 Dashboard Preview

![Superstore Dashboard]("C:\Users\Kartik\Downloads\Screenshot_22-5-2026_12163_.jpeg")

---

## 📬 Connect With Me

If you found this project helpful or have feedback, feel free to connect!

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/your-profile)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/your-username)

---

⭐ **If you found this project useful, please give it a star!**

---

*Built with 💙 using Power BI | Data cleaned in Power Query | Measures written in DAX*
