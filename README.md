<div align="center">

# <span style="color:#0E8DF2">KS</span> Adventure Works — Sales Dashboard

### Power BI · SQL · Python · Excel

[![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com)
[![SQL](https://img.shields.io/badge/SQL-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)](https://www.microsoft.com/sql-server)
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)](https://microsoft.com/excel)

> **A full-stack business intelligence solution** transforming raw Adventure Works sales data into interactive, decision-ready dashboards — covering revenue trends, customer analytics, product performance, and global market distribution.

</div>

---

## 📊 Live Dashboard Preview

> ▶️ **[View Interactive Dashboard](https://ris005.github.io/Mobile-Sales-Dashboard/)** — 5-page Power BI replica with auto-slide, region maps & animated KPIs

| Page | Focus |
|------|-------|
| 🏠 **Sales Overview** | $25M revenue, 56K orders, $10M profit, 2.17% return rate |
| 👥 **Customer Analytics** | 11K unique customers, revenue per customer trend, Top 100 table |
| 🗺️ **North America** | US vs Canada order distribution on interactive map |
| 🌍 **Europe** | UK, Germany, France order bubbles on Azure map |
| 📈 **Trending Matrix** | Monthly Orders / Revenue / Profit vs targets (gauge KPIs) |

---

## 🎯 Key Business Insights

```
💰  Total Revenue     →  $25M   (3× growth from 2020 to 2023)
📦  Total Orders      →  56K    (+0.26% MoM growth, Jan 2023)
📈  Total Profit      →  $10M   (40% profit margin)
🔁  Return Rate       →  2.17%  (well below 5% industry benchmark)
👤  Monthly Revenue   →  $1.83M (+3.31% vs prev month)
🧑  Unique Customers  →  11K    (FY 2022)
```

---

## 🛠️ Tech Stack

| Layer | Tool | Purpose |
|-------|------|---------|
| **Visualization** | Power BI Desktop | 5-page interactive dashboard, DAX measures |
| **Data Layer** | SQL Server / PostgreSQL | Data extraction, joins, aggregations |
| **Processing** | Python (Pandas, NumPy) | Data cleaning, EDA, transformation |
| **Pre-processing** | Microsoft Excel | Raw data formatting, validation |
| **Maps** | Azure Maps (Power BI) | Geographic order distribution |
| **Web Preview** | HTML / SVG / CSS | Pixel-accurate dashboard replica |

---

## 📁 Project Structure

```
Mobile-Sales-Dashboard/
│
├── 📊 PowerBI/
│   └── KS_Sales_Dashboard.pbix        # Main Power BI file (5 pages)
│
├── 🗄️ SQL/
│   ├── data_extraction.sql             # Main query — joins all fact/dim tables
│   ├── kpi_measures.sql                # Revenue, profit, return rate queries
│   └── customer_segmentation.sql       # Top 100 customers, occupation split
│
├── 🐍 Python/
│   ├── data_cleaning.py                # Null handling, type casting, dedup
│   ├── eda_analysis.py                 # Exploratory data analysis + plots
│   └── requirements.txt               # pandas, numpy, matplotlib, seaborn
│
├── 📂 Data/
│   ├── raw/                            # Source CSVs (Adventure Works dataset)
│   └── processed/                      # Cleaned, analysis-ready data
│
├── 📸 Screenshots/
│   ├── 00001_sales_overview.png
│   ├── 00002_customer_analytics.png
│   ├── 00003_north_america_map.png
│   ├── 00004_europe_map.png
│   └── 00005_trending_matrix.png
│
└── 🌐 Document_from_Rishu_Anand.html   # Interactive web preview
```

---

## 📸 Dashboard Screenshots

### Page 1 — Sales Overview
![Sales Overview](Screenshots/00001_sales_overview.png)
> Executive KPIs, revenue trend (2020–2023 with forecast), category donut, product table, and monthly mini-cards.

### Page 2 — Customer Analytics
![Customer Analytics](Screenshots/00002_customer_analytics.png)
> 11K unique customers, $9M revenue, revenue-per-customer trend, occupation breakdown, Top 100 table.

### Page 3 — North America Map
![North America](Screenshots/00003_north_america_map.png)
> Bubble map showing US (dominant) and Canada order distribution — US drives 80%+ of NA orders.

### Page 4 — Europe Map
![Europe](Screenshots/00004_europe_map.png)
> UK leads European sales, followed by Germany and France. Bubble size = order volume.

### Page 5 — Trending Matrix & Gauge KPIs
![Trending Matrix](Screenshots/00005_trending_matrix.png)
> Monthly performance vs targets: Orders at 91% (5,430 / 5,958), Revenue at 100% ($2M), Profit at 93.5% ($772K / $826K).

---

## ⚙️ Dashboard Pages — Detailed Breakdown

### 🏠 Page 1: Sales Overview
- **KPI Cards** — Total Revenue ($25M), Total Orders (56K), Total Profit ($10M), Return Rate (2.17%)
- **Revenue Line Chart** — Monthly trend Jan 2020 → Jan 2023 with forecast cone and trend line
- **Orders by Category** — Donut: Bikes 59.9%, Clothing 24.85%, Accessories 15.18%
- **Product Table** — Revenue + orders per SKU with inline data bars (pink = revenue, blue = orders)
- **Monthly Mini-Cards** — Monthly Revenue $1.83M (+3.31%), Orders 5.43K (+0.26%), Returns 166 (−1.78%)

### 👥 Page 2: Customer Analytics (2022)
- **Year Tabs** — Toggle between 2020, 2021, 2022 views
- **Revenue Per Customer Trend** — Jan–Jun 2022, trending from ₹720 → ₹860 with regression line
- **Occupation Donut** — Professional (teal), Skilled Manual (black), Management (gold)
- **Top 100 Customers Table** — Ranked by revenue; Mr. Jordan Turner leads at $6,802 / 13 orders
- **Smart Insight** — "Among Skilled Manual customers, Mr. Franklin Xu drove the most revenue"

### 🗺️ Pages 3 & 4: Geographic Maps
- **Region Tabs** — Toggle Europe / North America / Pacific
- **Azure Bubble Map** — Dot size proportional to order volume by country
- **Countries covered** — UK, Germany, France (Europe); United States, Canada (North America)

### 📈 Page 5: Trending Matrix
- **Gauge KPIs** — Orders vs target (5,430 / 5,958), Revenue vs target ($2M / $2M), Profit vs target ($772K / $826K)
- **Multi-line trend** — Total Orders (blue), Total Revenue (navy), Total Profit (orange), Return Rate (magenta flat)
- **Product + Metric Slicers** — Filter by product name or metric type
- **Date Range Slider** — Jan 2020 → Jan 2022

---

## 🚀 Getting Started

### Prerequisites
```bash
# Python dependencies
pip install pandas numpy matplotlib seaborn openpyxl

# Or install all at once
pip install -r Python/requirements.txt
```

### Run Data Cleaning
```bash
cd Python/
python data_cleaning.py
# Output: ../Data/processed/adventure_works_clean.csv
```

### Run EDA
```bash
python eda_analysis.py
# Generates plots in ../Screenshots/eda/
```

### SQL — Extract Data
```sql
-- Run in SQL Server / PostgreSQL
-- Main extraction query
\i SQL/data_extraction.sql

-- KPI measures
\i SQL/kpi_measures.sql
```

### Open Dashboard
1. Download `PowerBI/KS_Sales_Dashboard.pbix`
2. Open in **Power BI Desktop** (free download from Microsoft)
3. If prompted, update the data source path to your local `Data/processed/` folder
4. Refresh data → all visuals update automatically

---

## 📐 Key DAX Measures

```dax
-- Total Revenue
Total Revenue = SUM(Sales[SalesAmount])

-- Profit Margin %
Profit Margin = DIVIDE([Total Profit], [Total Revenue], 0)

-- Return Rate
Return Rate = DIVIDE([Total Returns], [Total Orders], 0)

-- Revenue vs Prior Month
Rev MoM % = 
DIVIDE(
    [Total Revenue] - CALCULATE([Total Revenue], DATEADD('Calendar'[Date], -1, MONTH)),
    CALCULATE([Total Revenue], DATEADD('Calendar'[Date], -1, MONTH)),
    0
)

-- Revenue Per Customer
Rev Per Customer = DIVIDE([Total Revenue], DISTINCTCOUNT(Sales[CustomerKey]), 0)

-- Monthly Orders vs Target
Orders vs Target = [Total Orders] - [Order Target]
```

---

## 📊 Dataset — Adventure Works

| Table | Rows | Description |
|-------|------|-------------|
| `FactInternetSales` | ~60K | Core transaction data |
| `DimCustomer` | ~11K | Customer demographics & geography |
| `DimProduct` | ~300 | Product catalog with categories |
| `DimDate` | ~1,400 | Calendar table for time intelligence |
| `DimSalesTerritory` | 10 | Europe / North America / Pacific regions |
| `DimEmployee` | ~290 | Sales rep assignments |

> Adventure Works is Microsoft's sample retail dataset for a fictional cycling products company. [Download here](https://learn.microsoft.com/en-us/sql/samples/adventureworks-install-configure)

---

## 💡 What I Learned / Built

- ✅ Designed a **5-page Power BI report** from scratch with consistent dark/light theme
- ✅ Built **custom DAX measures** for MoM%, YoY, Return Rate, and Revenue Per Customer
- ✅ Used **Azure Maps visual** with bubble sizing by order volume across 3 regions
- ✅ Created **forecast cones** and trend lines on revenue charts
- ✅ Built a **pixel-accurate HTML replica** of the dashboard for web preview (no Power BI license needed to view)
- ✅ Applied **data bars inside table cells** using conditional formatting
- ✅ Wrote **SQL queries** for data extraction and KPI pre-aggregation
- ✅ Used **Pandas** for data cleaning — null handling, type casting, outlier detection

---

## 🔗 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/rishu-anand)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Ris005)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white)](https://ris005.github.io)

---

<div align="center">

**⭐ Star this repo if you found it useful!**

*Built by [Rishu Anand](https://github.com/Ris005) — ECE @ VIT | AI/ML & Data Science*

</div>
