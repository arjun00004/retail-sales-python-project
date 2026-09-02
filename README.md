# 🛒 Retail Sales Data Analysis

**Exploratory Data Analysis & Business Insights using Python (NumPy, Pandas, Matplotlib, Seaborn)**

A beginner-to-intermediate Data Analyst portfolio project that cleans, explores, and visualizes retail sales data to uncover actionable business insights — top categories, regional performance, seasonal trends, and the impact of discounts on profitability.

---

## 📌 Project Overview

This project analyzes a retail sales dataset (**1,210 orders**, spanning **Jan 2024 – Dec 2025**) to answer real business questions such as:

- Which product categories and regions drive the most revenue?
- How do sales trend month over month?
- Which customer segments are most profitable?
- Does offering a discount actually hurt profit margins?

The workflow follows a standard data analytics pipeline: **Load → Clean → Explore (EDA) → Visualize → Summarize Insights.**

---

## 🧰 Tech Stack

| Tool | Purpose |
|------|---------|
| **Python** | Core programming language |
| **NumPy** | Numerical computations & array-based summary statistics |
| **Pandas** | Data cleaning, grouping, and aggregation |
| **Matplotlib** | Base plotting |
| **Seaborn** | Statistical visualizations & styling |

---

## 📂 Dataset

`retail_sales_data.csv` — 1,210 records with the following fields:

`OrderID`, `OrderDate`, `CustomerID`, `CustomerSegment`, `Region`, `ProductCategory`, `Product`, `Quantity`, `UnitPrice`, `DiscountPct`, `Sales`, `Profit`, `ShippingCost`, `PaymentMode`

---

## 🧹 Data Cleaning

- Filled missing `DiscountPct` values with `0` (assumed no discount applied)
- Removed duplicate orders based on `OrderID`
- Engineered new columns: `Month` (for trend analysis) and `ProfitMargin` (Profit ÷ Sales × 100)
- Verified data types and checked for remaining missing values

---

## 📊 Key Visualizations

| # | Chart | Insight |
|---|-------|---------|
| 1 | **Sales by Category** (Bar) | Electronics dominates total revenue, followed by Furniture |
| 2 | **Monthly Sales Trend** (Line) | Reveals seasonal spikes and dips across 2024–2025 |
| 3 | **Sales Distribution** (Histogram) | Most orders are low-to-mid value, with a long right tail of high-ticket sales |
| 4 | **Region × Category Heatmap** | Electronics leads in every region; West & East are the strongest markets |
| 5 | **Profit Margin by Segment** (Boxplot) | Home Office customers show the highest median profit margin |
| 6 | **Discount % vs Profit** (Scatter) | Higher discounts are associated with shrinking, sometimes negative, profit |

*(See the `/charts` folder for all generated PNGs.)*

---

## 💡 Key Business Insights

- 🏆 **Best-selling category:** Electronics
- 🌍 **Top-performing region:** West
- 💰 **Most profitable customer segment (avg. profit):** Home Office
- 📦 **Best-selling product:** Identified via top-5 product analysis
- 📉 **Loss-making orders:** A measurable share of orders are unprofitable, concentrated at higher discount levels

> Full printed insights are generated automatically when running the script (see below).

---

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/retail-sales-analysis.git
   cd retail-sales-analysis
   ```

2. Install dependencies:
   ```bash
   pip install numpy pandas matplotlib seaborn
   ```

3. Make sure `retail_sales_data.csv` is in the same folder as the script, then run:
   ```bash
   python retail_sales_analysis.py
   ```

4. The script will print step-by-step analysis in the terminal and save **6 charts** as PNG files in the project folder.

---

## 📁 Project Structure

```
retail-sales-analysis/
│
├── retail_sales_analysis.py       # Main analysis script
├── retail_sales_data.csv          # Dataset
├── README.md                      # Project documentation
└── charts/
    ├── chart1_sales_by_category.png
    ├── chart2_monthly_sales_trend.png
    ├── chart3_sales_distribution.png
    ├── chart4_region_category_heatmap.png
    ├── chart5_profit_margin_boxplot.png
    └── chart6_discount_vs_profit.png
```

---

## 🔮 Future Improvements

- Build an interactive dashboard (Power BI / Tableau / Streamlit)
- Add time-series forecasting for future sales
- Perform customer segmentation (RFM analysis)
- Deploy insights as a web app for stakeholders

---

## 👤 Author

**Nithyanandham**
Aspiring Data Analyst | Electronics & Communication Engineering background
📫 Connect with me on [LinkedIn](#) | [GitHub](#)

---

⭐ If you found this project useful, consider giving it a star on GitHub!
