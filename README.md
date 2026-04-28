# 🚗 Bright Motors — Car Sales Analysis

> **BrightLearn Data Analytics Case Study**
> Role: Junior Data Analyst | Dataset: Bright Car Sales

---

## 📋 Project Overview

This project analyses historical car sales data for **Bright Motors**, a dealership looking to expand its network and improve sales performance. The analysis was prepared to support the newly appointed Head of Sales with actionable insights and data-driven recommendations.

---

## 🎯 Objectives

- Identify which car makes and models generate the most revenue
- Explore the relationship between price, mileage, and year of manufacture
- Determine which regions or locations have the highest sales volumes
- Uncover emerging trends in customer purchasing preferences
- Provide recommendations to increase dealership profitability and efficiency

---

## 🗂️ Project Structure

```
bright-motors-analysis/
│
├── architecture/
│   └── data_architecture_diagram.png       # Data flow & pipeline diagram (Task 1)
│
├── data/
│   ├── bright_car_sales.xlsx               # Raw dataset
│   └── car_sales_processed.xlsx            # Cleaned & transformed dataset (Task 2)
│
├── sql/
│   └── car_sales_queries.sql               # All SQL scripts used in DataBricks (Task 2)
│
├── presentation/
│   └── BrightMotors_Presentation.pdf       # Final presentation for Head of Sales (Task 4)
│
└── README.md
```

---

## 🔧 Tools & Technologies

| Category         | Tools Used                                              |
|------------------|---------------------------------------------------------|
| Coding / SQL     | DataBricks / MySQL / BigQuery / SQL Server               |
| Visualization    | Microsoft Excel / Power BI / Google Looker Studio       |
| Presentation     | Microsoft PowerPoint / Canva                            |
| Project Planning | Miro                                            |

---

## 📐 Data Architecture

The data pipeline follows this flow:

```
[Source: Excel/CSV Dataset]
        ↓
[ETL Pipeline]
  • Remove duplicates
  • Handle missing values
  • Format currencies to numeric
        ↓
[Storage: DataBricks / SQL Database]
        ↓
[Analysis Layer: SQL + Excel / Power BI]
        ↓
[Presentation Layer: PowerPoint / Canva]
```

---

## 🔑 Key Calculations

| Metric           | Formula                                                        |
|------------------|----------------------------------------------------------------|
| `Total_Revenue`  | `Selling_Price × Units_Sold`                                   |
| `Profit_Margin`  | `(Selling_Price − Cost_Price) ÷ Selling_Price × 100`          |
| **Grouping By**  | Make, Model, Year, Region, Fuel_Type                          |

---

## ✅ Tasks Summary

### Task 1 — Planning & Architecture
- Created a data flow diagram outlining the full pipeline from source to presentation
- Mapped key insights to deliver and grouped key calculations

### Task 2 — Data Processing (DataBricks / SQL)
- Converted Excel dataset to CSV and loaded into SQL platform
- Cleaned data: removed duplicates, converted text-based prices to numeric
- Engineered new columns: `total_revenue`, `profit_margin`
- Categorised cars into performance tiers: **High Margin**, **Medium Margin**, **Low Margin**
- Grouped transactions by month, quarter, and year

### Task 3 — Data Analysis & Visualisation
- Exported processed data to Excel / Power BI
- Built interactive dashboards with slicers for **Region**, **Fuel Type**, and **Year**
- Visualised revenue by make/model, regional performance, and price trends over time

### Task 4 — Presentation
- Prepared a professional, concise presentation summarising findings and strategic recommendations for the Head of Sales

---

## 📦 Deliverables

| # | File | Description |
|---|------|-------------|
| 1 | `data_architecture_diagram.png` | Miro / Architecture Diagram |
| 2 | `car_sales_processed.xlsx` | Cleaned & transformed dataset |
| 3 | `BrightMotors_Presentation.pdf` | Final stakeholder presentation |
| 4 | `car_sales_queries.sql` | All SQL scripts used |

---

## 💡 Notes

- All prices must be in numeric format (no commas or currency symbols)
- Missing or inconsistent values are handled during the ETL stage
- Column names in SQL are standardised and consistent (snake_case)
- Dashboards include short insight annotations for stakeholder clarity

---

