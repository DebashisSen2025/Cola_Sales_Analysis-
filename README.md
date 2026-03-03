# 🥤 Coca-Cola Sales Analysis | Retail Performance Analytics Project

> End-to-end sales performance analysis of Coca-Cola retail data to uncover
> revenue trends, regional performance, product insights, and profitability drivers.
> This project demonstrates strong data cleaning, aggregation, and business analytics skills.

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Excel](https://img.shields.io/badge/Dataset-Excel-green?style=for-the-badge)
![Matplotlib](https://img.shields.io/badge/Visualization-Matplotlib-orange?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

---

## 📌 Project Overview

| Detail        | Info |
|---------------|------|
| Tool          | Python (Jupyter Notebook) |
| Dataset       | Coke-sales-analysis-solution20.xlsx |
| Domain        | Retail / FMCG Analytics |
| Techniques    | Data Cleaning, Aggregation, KPI Analysis |
| Records       | 3,892+ sales transactions |
| Status        | ✅ Completed |

---

## 🎯 Business Questions Answered

- ✅ Which beverage brand generates the highest revenue?
- ✅ Which region contributes the most total sales?
- ✅ What is the monthly sales trend?
- ✅ Which retailer performs best in terms of revenue?
- ✅ What is the average operating margin?
- ✅ Which state has the highest profitability?

---

## 🔍 Key Analysis Performed

### 📊 Sales Performance Analysis
- Total Revenue Calculation
- Units Sold Analysis
- Monthly Sales Trend
- Revenue by Beverage Brand

### 🌍 Regional Performance
- Region-wise Sales Distribution
- State-wise Profit Comparison
- City-level Revenue Insights

### 🏪 Retailer Analysis
- Top Performing Retailers
- Revenue vs Profit Comparison
- Operating Margin Evaluation

### 📋 Data Cleaning Applied
- Removed empty rows
- Renamed columns properly
- Converted invoice date to datetime format
- Extracted month from invoice date
- Verified numeric columns (Sales, Profit, Units)

---

## 🧮 Sample Python Code

```python
import pandas as pd

# Load dataset
df = pd.read_excel("Coke-sales-analysis-solution20.xlsx")

# Total Revenue
total_sales = df["Total Sales"].sum()

# Region-wise Sales
region_sales = df.groupby("Region")["Total Sales"].sum().sort_values(ascending=False)

# Monthly Sales Trend
df["Invoice Date"] = pd.to_datetime(df["Invoice Date"])
monthly_sales = df.groupby(df["Invoice Date"].dt.month)["Total Sales"].sum()

# Top 5 Retailers
top_retailers = df.groupby("Retailer")["Total Sales"] \
                   .sum() \
                   .sort_values(ascending=False) \
                   .head(5)
```

---

## 📈 Key Insights

- Certain regions dominate total revenue contribution.
- A small number of retailers drive significant sales volume.
- Monthly sales show seasonal demand fluctuations.
- Operating margin varies significantly across states.
- Some brands perform strongly in specific regions.

---

## 📂 Project Structure

```
├── Cola_Sales_Analysis.ipynb
├── Coke-sales-analysis-solution20.xlsx
└── README.md
```

---

## ▶️ How to Run

1️⃣ Install Python 3.8+  
2️⃣ Install required libraries

```bash
pip install pandas matplotlib seaborn openpyxl
```

3️⃣ Open Jupyter Notebook

```bash
jupyter notebook
```

4️⃣ Run the notebook step-by-step

---

## 🧠 Skills Demonstrated

- Exploratory Data Analysis (EDA)
- Retail KPI Analysis
- Business Insight Extraction
- Data Cleaning & Transformation
- Data Visualization
- Profitability & Margin Analysis

---

## 👋 About Me

**Debashis Sen** | Aspiring Data Analyst  

🏆 HackerRank SQL — 5 Star  
📊 Multiple Real-World Analytics Projects  
📍 Jamshedpur, India | Immediate Joiner  

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Debashis_Sen-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/debashis-sen25)
[![GitHub](https://img.shields.io/badge/GitHub-DebashisSen2025-black?style=flat&logo=github)](https://github.com/DebashisSen2025)

---

⭐ If you found this project useful, please give it a star!
