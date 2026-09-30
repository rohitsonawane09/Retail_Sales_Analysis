# 📊 Retail Sales Analysis Using Python

## 📌 Project Overview

This project is an exploratory analysis of retail sales data using **Python, Pandas, NumPy, and Matplotlib**.

The objective is to analyze sales and profitability patterns across products, customers, categories, regions, shipping modes, and time periods, while answering practical business questions from the data.

This project was built as my **first end-to-end Data Analyst project** to develop practical skills in data cleaning, exploratory data analysis, time-series analysis, and business-oriented data interpretation.

---

## 🎯 Business Objective

The analysis focuses on understanding the following areas:

- Which categories and sub-categories contribute most to sales and profit?
- Which products and customers generate the highest sales and profit?
- How does performance vary across regions and states?
- How does shipping mode relate to shipping time?
- How do sales change over time?
- Are there noticeable seasonal patterns?
- How are discounts associated with profitability?
- Which areas may require further business investigation?

---

## 🗂️ Dataset

The project uses a retail sales dataset containing information about:

- Orders
- Customers
- Products
- Categories and sub-categories
- Sales
- Profit
- Discounts
- Regions and states
- Shipping modes
- Order and shipping dates

### Dataset Grain

Each row represents an **order-line record**. A single `Order_ID` can appear across multiple rows when an order contains multiple products.

Therefore, analyses based directly on DataFrame rows are interpreted as **order-line analysis** unless the data is first aggregated to the order level.

> The original dataset is not included in this repository because of its file size.

---

## 🛠️ Tools & Technologies

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Jupyter Notebook**

---

## 🔍 Analytical Workflow

The project follows a practical data-analysis workflow:

### 1. Data Understanding

- Inspected dataset dimensions
- Reviewed columns and data types
- Examined categorical and numerical variables
- Identified the dataset grain

### 2. Data Cleaning

- Checked for missing values
- Checked for duplicate rows
- Converted date columns to appropriate datetime format
- Standardized column names where required
- Prepared the dataset for analysis

### 3. Exploratory Data Analysis

Analyzed:

- Sales performance
- Profitability
- Categories and sub-categories
- Products
- Customers
- Regions and states
- Shipping modes
- Discounts

### 4. Time-Series Analysis

Performed:

- Monthly sales analysis
- Quarterly sales analysis
- Yearly sales analysis
- Year-over-year growth analysis
- Month-over-month growth analysis
- 30-day rolling average analysis
- Seasonality analysis

### 5. Business Analysis

The analysis uses business questions to transform raw data into interpretable findings and potential areas for further investigation.

---

## 📈 Key Findings

The analysis identified several notable patterns:

### Category & Product Performance

- Technology is a strong contributor to both sales and profitability.
- Copiers and Phones are among the stronger-performing sub-categories.
- Tables and Bookcases generate sales but show negative total profit in the analyzed data.
- A relatively small number of products contribute a substantial share of total profit.

### Customer Performance

- A small group of customers contributes a significant share of total sales.
- High-value customers can be further analyzed using purchase frequency, recency, and profitability.

### Regional Performance

- Sales and profitability vary considerably across states and regions.
- The West region shows strong overall profitability in the analyzed dataset.

### Shipping Performance

- Shipping time differs substantially between shipping modes.
- Standard Class has the longest average shipping time, while faster shipping modes have shorter delivery times.

### Sales Trends & Seasonality

- Sales show noticeable seasonal patterns.
- Q4 generally records stronger sales than several other periods.
- Annual sales declined slightly in 2015 before increasing strongly in 2016 and 2017.
- The 30-day rolling average reduces short-term variability and makes broader sales patterns easier to observe.

### Discounts & Profitability

- Higher discount levels are associated with lower profitability and a higher proportion of loss-making order-line records.
- This indicates an area that could be investigated further by category and product.

> These findings describe patterns observed in the dataset and should not automatically be interpreted as causal relationships.

---

## 💡 Business Recommendations

Based on the analysis, the following areas were identified for further business investigation:

### 1. Plan Operations Around Q4 Seasonality

Historical sales patterns indicate stronger demand during Q4.

**Recommendation:** Use historical seasonal patterns to support inventory, staffing, and fulfillment planning before peak periods.

### 2. Investigate Furniture Profitability

Tables and Bookcases generate sales but show negative total profit.

**Recommendation:** Review pricing, discounts, costs, and product mix before making changes to the discount strategy.

### 3. Evaluate Technology Performance

Technology is an important contributor to overall sales and profitability.

**Recommendation:** Review high-performing Technology products and sub-categories for potential inventory and marketing opportunities.

### 4. Investigate High-Discount Transactions

Higher discount levels are associated with weaker profitability.

**Recommendation:** Analyze high-discount transactions by category and product before changing discount policies.

### 5. Further Analyze High-Value Customers

A relatively small group of customers contributes a substantial share of sales.

**Recommendation:** Analyze customer frequency, recency, and profitability before designing targeted retention strategies.

---

## 📚 Key Learnings

This project helped me develop practical experience with:

- Working with Pandas DataFrames
- Data cleaning and preprocessing
- Handling missing values
- Checking duplicate records
- Data type conversion
- Filtering and sorting data
- `groupby()` and aggregation
- `pivot_table()`
- NumPy array operations
- Date and time analysis
- Resampling time-series data
- Rolling averages
- Percentage change
- Exploratory Data Analysis
- Asking business questions from data
- Translating analytical findings into business insights
- Communicating analytical results clearly

---

## 📁 Repository Structure

```text
retail-sales-analysis/
│
├── Retail_Sales_Analysis.ipynb
├── README.md
├── requirements.txt
│
└── data/
    └── README.md
