# 📊 AtliQ Hardwares – Business Intelligence Report (Excel)

<p align="center">
  <img src="https://img.shields.io/badge/Tool-Microsoft%20Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white"/>
  <img src="https://img.shields.io/badge/Technique-Pivot%20Tables-F5A623?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Feature-Power%20Query-0078D4?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Feature-Power%20Pivot-107C41?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge"/>
</p>

---

## 🏢 About the Project

> **AtliQ Hardwares** is a consumer electronics company that sells hardware products (PCs, peripherals, networking gear, accessories) across multiple regions globally.

This project delivers a **multi-sheet Excel Business Intelligence Report** that enables leadership to analyse sales performance across divisions, products, and geographies — comparing **2020 vs 2021** to drive data-backed decisions.

---

## 🎯 Business Problem

AtliQ Hardwares lacked a consolidated, filterable view of their sales data. The management needed answers to:

- Which **divisions** are growing and by how much?
- What are the **Top 10 and Bottom 5** products by quantity sold?
- Which **new products** launched in 2021 are gaining traction?
- Which **countries** are the highest revenue contributors in 2021?

---

## 📁 Report Sheets Overview

### 1. 🏆 Top 10 Products
> *Sheet: `Top 10 products`*

Displays the **top 10 products by net sales** for 2020 and 2021, with a **21 vs 20 % growth column** and colour-coded data bars for quick visual comparison.

| Highlight | Value |
|-----------|-------|
| Grand Total 2020 | 6.4M USD |
| Grand Total 2021 | 52.0M USD |
| Overall Growth | **708%** |
| Top Product Growth | AQ LION x3 — **1692.3%** |

---

### 2. 📂 Division Level Report
> *Sheet: `Division`*

Breaks down net sales by **division** (N&S, P&A, PC) with 2020 vs 2021 comparison and percentage growth. Filterable by **region** and **customer**.

| Division | 2020 | 2021 | Growth |
|----------|------|------|--------|
| N & S | 51.4M | 94.7M | 84.1% |
| P & A | 105.2M | 338.4M | 221.5% |
| PC | 40.1M | 165.8M | 313.7% |
| **Grand Total** | **196.7M** | **598.9M** | **204.5%** |

---

### 3. 📦 Top & Bottom Products – QTY
> *Sheet: `Top and bottom products - QTY`*

Two tables in one sheet showing:
- **Top 5 products** by quantity sold (led by AQ Master wired x1 Ms — 4.2M units)
- **Bottom 5 products** by quantity sold (lowest: AQ HOME Allin1 Gen 2 — 8.9K units)

Filtered independently by region, division, and customer.

---

### 4. 🆕 New Products – 2021
> *Sheet: `New products - 2021`*

Lists all **products introduced in 2021** that had zero sales in 2020, showing their 2021 net revenue. Filterable by region, division, and customer.

| Highlight | Value |
|-----------|-------|
| Total New Products | 16 |
| Grand Total Revenue | **176.2M USD** |
| Top New Product | AQ Qwerty — 22.0M |

---

### 5. 🌍 Top 5 Countries – 2021
> *Sheet: `Top 5 countries`*

Ranks the **top 5 countries by net sales in 2021**. Filterable by region and customer.

| Country | 2021 Net Sales |
|---------|---------------|
| India | **161.3M** |
| USA | 87.8M |
| South Korea | 49.0M |
| United Kingdom | 34.2M |
| Canada | 35.1M |
| **Grand Total** | **367.2M** |

---

## 🛠️ Tools & Techniques Used

| Tool / Feature | Purpose |
|----------------|---------|
| **Power Query** | Data cleaning, transformation, merging tables |
| **Power Pivot** | Data modelling, creating relationships across tables |
| **Pivot Tables** | Dynamic aggregation and summarisation |
| **Slicers / Filters** | Interactive filtering by region, division, customer |
| **Conditional Formatting** | Data bars and colour highlights for visual impact |
| **DAX Measures** | Custom KPIs like 21 vs 20 % growth |

---

## 📐 Data Model

```
fact_sales_monthly
    ├── dim_product     (product_code → segment, division, category)
    ├── dim_customer    (customer_code → customer, market, region, sub_zone)
    └── dim_date        (date → month, year, fiscal_year)
```

---

## 💡 Key Insights

- 📈 **Overall company net sales grew 204.5%** from 2020 to 2021 (196.7M → 598.9M USD)
- 💻 The **PC division** saw the highest growth at **313.7%**
- 🇮🇳 **India** is the single largest market at 161.3M USD in 2021
- 🆕 **16 new products** were launched in 2021, collectively generating **176.2M USD**
- 🏅 **AQ Master wired x1 Ms** is the highest-selling product by quantity at **4.2M units**
- ⚠️ **AQ HOME Allin1 Gen 2** is the weakest product with only **8.9K units** sold

---

## 📂 File Structure

```
📦 AtliQ-Hardwares-Excel-Report
 ┣ 📊 Business_Solution.xlsx       ← Main report workbook
 ┣ 📁 screenshots/
 ┃  ┣ 🖼️ top_10_products.png
 ┃  ┣ 🖼️ division_report.png
 ┃  ┣ 🖼️ top_bottom_qty.png
 ┃  ┣ 🖼️ new_products_2021.png
 ┃  ┣ 🖼️ top_5_countries.png
 ┗ 📄 README.md
```

---

## 🚀 How to Use

1. **Download** `Business_Solution.xlsx`
2. Open in **Microsoft Excel 2016+** or **Microsoft 365**
3. If prompted, click **Enable Editing** and **Enable Content**
4. Navigate between sheets using the tabs at the bottom
5. Use the **FILTERS** slicers on each sheet to drill down by region, division, or customer

---

## 👨‍💻 Author

**Saurabh Gautam Hanwate**
M.Sc. Computational Modeling & Simulation (Applied AI) — TU Dresden

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin)](https://linkedin.com/in/saurabh-hanwate)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=flat&logo=github)](https://github.com/SaurabhHanwate)

---

> *"Without data, you're just another person with an opinion." — W. Edwards Deming*
