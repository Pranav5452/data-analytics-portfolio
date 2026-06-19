# 🚲 Bike Sales Analysis — Excel Dashboard Project

An end-to-end data analysis project built in Microsoft Excel, exploring the demographic and behavioral factors that influence bike purchase decisions across 1,000 customers.

---

## 📌 Project Overview

This project simulates a real-world business scenario: a bike retailer wants to understand **who is buying bikes and why**, so they can target marketing more effectively. Starting from raw customer data, I cleaned and transformed the dataset, built pivot table analyses across three key dimensions, and delivered an interactive dashboard with slicers for dynamic filtering.

---

## 🗂️ Dataset

| Field | Description |
|---|---|
| ID | Unique customer identifier |
| Marital Status | Married / Single |
| Gender | Male / Female |
| Income | Annual income in EUR |
| Children | Number of children |
| Education | Highest education level |
| Occupation | Job category |
| Home Owner | Yes / No |
| Cars | Number of cars owned |
| Commute Distance | Distance band (0-1 Miles → 10 Miles+) |
| Region | Europe / Pacific |
| Age | Customer age |
| Age Brackets | Derived column (Adolescent / Middle Age / Old) |
| Purchased Bike | Target variable — Yes / No |

**1,000 rows · 14 columns · EUR income values**

---

## 🔧 Process

### 1. Data Cleaning (Working Sheet)
- Removed duplicate records
- Standardised categorical values (e.g. consistent capitalisation)
- Checked for blanks and nulls across all columns
- **Engineered the `Age Brackets` column** using a nested `IF` formula to group customers into Adolescent, Middle Age, and Old segments

### 2. Pivot Table Analysis (3 Tables)
Built three separate pivot tables to explore different angles of the purchase decision:

**① Average Income Per Purchase — by Gender**
- Compared average income of buyers vs non-buyers, split by gender
- Males who purchased: **€60,124 avg income** vs €56,208 for non-buyers
- Females who purchased: **€55,774 avg income** vs €53,440 for non-buyers

**② Customer Commute Distance vs Purchase Count**
- Counted buyers and non-buyers across 5 commute distance bands
- Strongest purchase volume at **0-1 Miles (200 buyers)**
- Sharpest drop-off at **10 Miles+ (only 33 buyers)**

**③ Customer Age Bracket vs Purchase Count**
- **Middle Age** dominated purchases (383 Yes out of 701)
- **Old** customers had the lowest conversion (59 Yes out of 189)
- **Adolescents** showed relatively stronger purchase rate for their group size (39 Yes out of 110)

### 3. Interactive Dashboard
- 3 PivotCharts connected to all 3 pivot tables
- **3 Slicers:** Marital Status · Gender · Occupation
- Selecting any slicer value filters all charts simultaneously
- Clean layout with a dark title banner

---

## 📊 Key Insights

> **1. Income is a purchase signal — especially for men.**
> Male buyers earn ~€4,000 more on average than male non-buyers. The income gap exists for females too, but is slightly smaller.

> **2. Short-commute customers are the highest-converting segment.**
> Customers commuting 0-1 miles are 6× more likely to buy than those commuting 10+ miles — likely using bikes for their daily commute.

> **3. Middle Age is the core buyer demographic.**
> 383 of 481 total buyers fall in the Middle Age bracket. Marketing should be concentrated here, while adolescents represent an emerging segment worth developing.

---

## 🛠️ Tools Used

- **Microsoft Excel** — Data Cleaning, Feature Engineering, Pivot Tables, PivotCharts, Slicers, Dashboard Design

---

## 📁 File Structure

```
bike-sales-excel/
│
├── Excel_Project.xlsx        # Main workbook
│   ├── bike_buyers           # Raw source data
│   ├── Working Sheet         # Cleaned + transformed data
│   ├── Pivot Table           # Three pivot tables + charts
│   └── Dashboard             # Interactive dashboard with slicers
│
├── screenshots/
│   ├── 01_raw_data.png
│   ├── 02_pivot_income.png
│   ├── 03_pivot_commute.png
│   ├── 04_pivot_age.png
│   └── 05_dashboard.png
│
└── README.md
```

---

## 📸 Screenshots

### Raw Data (Working Sheet)
> Cleaned dataset with 14 columns including the engineered Age Brackets column.

### Pivot Table — Average Income Per Purchase
> Income comparison by gender and purchase decision, with bar chart.

### Pivot Table — Customer Commute
> Purchase counts by commute distance band, showing steep drop-off at longer distances.

### Pivot Table — Customer Age Brackets
> Purchase distribution across Adolescent, Middle Age, and Old segments.

### Interactive Dashboard
> Full dashboard with all 3 charts and slicers for Marital Status, Gender, and Occupation.

---

## 💡 What I Learned

- How to structure a multi-sheet Excel project cleanly (raw → clean → analysis → dashboard)
- Building PivotCharts that respond dynamically to slicers across multiple pivot tables
- Translating raw numbers into a narrative: income, distance, and age each tell a different part of the purchase story
- Dashboard layout principles: consistent chart style, clear titles, slicer placement for usability

---
