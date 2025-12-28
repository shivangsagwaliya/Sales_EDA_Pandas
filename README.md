# 📊 Sales Data Analysis & EDA

A comprehensive Exploratory Data Analysis (EDA) project using Python to analyze 12 months of electronics sales data. This project transforms raw transactional data into actionable business insights, focusing on customer purchasing behavior, product performance, and optimal advertising strategies.

---

## 🚀 Project Overview

The goal of this project is to solve real-world business questions using data analysis. By cleaning and aggregating sales data from multiple sources, we derive insights that can help a retail business optimize its supply chain and marketing efforts.

### Key Business Questions Answered:
1. **Sales Trends:** What was the best month for sales, and how much was earned?
2. **City Analysis:** Which city sold the most products?
3. **Timing Optimization:** What is the best time to display advertisements to maximize customer likelihood of buying?
4. **Market Basket Analysis:** Which products are most often sold together?
5. **Price Sensitivity:** Is there a correlation between the price of a product and the quantity sold?

---

## 🛠️ Technologies Used

* **Python 3.x**
* **Pandas**: For data manipulation, concatenation, and cleaning.
* **Matplotlib & Seaborn**: For data visualization (bar charts, line graphs, and overlay plots).
* **Itertools & Collections**: For advanced counting in Market Basket Analysis.
* **OS Module**: For handling directory paths and batch file processing.

---

## 📂 Dataset

The dataset contains 12 CSV files (one for each month of sales data).
**Key Columns:**
* `Order ID`: Unique identifier for the transaction.
* `Product`: Name of the item sold.
* `Quantity Ordered`: Number of items in the order.
* `Price Each`: Cost per unit.
* `Order Date`: Timestamp of the purchase.
* `Purchase Address`: Shipping address (used to extract City/Zip Code).

---

## 📊 Key Analysis & Insights

### 1. Data Cleaning & Preparation
* Aggregated 12 separate CSV files into a single DataFrame using `os` and `pd.concat`.
* Handled missing values (`NaN`) and removed header duplicates found in the raw files.
* Converted data types (e.g., `Order Date` to datetime, numeric columns to integers/floats).
* **Feature Engineering**: Created new columns for `Month`, `City`, `Hour`, and `Revenue`.

### 2. Market Basket Analysis
Used `itertools.combinations` and `Counter` to identify product pairs frequently purchased together.
* *Insight Example:* `iPhone` and `Lightning Charging Cable` are among the most common pairs, suggesting a strong cross-selling opportunity.

### 3. Visualizations
* **Monthly Sales Revenue**: Bar charts analyzing seasonal trends.
* **Hourly Sales Distribution**: Line charts to pinpoint peak shopping hours (recommendation: advertise around 11 AM and 7 PM).
* **Product Volume vs. Price**: A dual-axis chart overlaying the quantity sold (bar) with the unit price (line) to visualize price sensitivity.

---

## 💻 How to Run

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/shivangsagwaliya/Sales_EDA_Pandas.git](https://github.com/shivangsagwaliya/Sales_EDA_Pandas.git)
