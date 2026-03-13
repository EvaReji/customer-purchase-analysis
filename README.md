# Customer-Purchase-Analysis-Project

Analyzing customer purchase behavior and product sales trends using Pandas, Matplotlib, and Seaborn.

## About This Project

This project explores an online retail dataset to understand customer purchasing patterns and overall sales performance.

It is being built step by step as part of my Data Analytics learning journey.

## Dataset

This project uses the **Online Retail dataset**, originally sourced from the UCI Machine Learning Repository and obtained via Kaggle.(https://archive.ics.uci.edu/ml/datasets/online+retail)

The dataset contains transactional data from a UK-based online retail store between 2010–2011.

It includes:

- Invoice numbers  
- Product (Stock) codes  
- Product descriptions  
- Quantities purchased  
- Unit prices  
- Customer IDs  
- Country information  

During data exploration, although the dataset documentation suggests no missing values, missing values were identified in certain columns and were handled appropriately during the data cleaning process.

The dataset is used to analyze customer purchasing behavior, sales trends, and overall revenue patterns.

## 🛠 Tools Used

- **Pandas** – for data cleaning, feature extraction, and analysis.  
- **Matplotlib** – for visualizations and charts.  
- **Seaborn** – for advanced and styled visualizations.  
- **Jupyter Notebook** – for step‑by‑step workflow, documentation, and analysis.  
- **VS Code** – for editing and managing code.  
- **Git** – for version control and maintaining a clean project history.  
- **GitHub** – for hosting projects, sharing progress, and recruiter visibility.  

## Day 1 - Basic Exploration

- Loaded the Online Retail dataset
- Explored dataset structure and data types
- Generated summary statistics
- Checked for missing values

## Day 2 – Data Cleaning & Preparation

- Removed missing values.  
- Removed negative quantity transactions (returns/cancellations).  
- Removed zero UnitPrice rows.  
- Removed duplicate records.  
- Converted **InvoiceDate** to datetime format.  
- Extracted new features: Year, Month, Weekday, Hour.  
- Created **TotalPrice** column (Quantity × UnitPrice).  
- Verified unique customers (4,338) and countries (37).  
- Fixed country name: replaced **EIRE** with **Ireland** for consistency.  

## Day 3 – Sales Insights & Visualization

- Identified top performing products, customers, and countries using sales data
- Calculated top 10 products by quantity sold
- Calculated top 10 products by revenue
- Identified top 10 customers by quantity purchased
- Analyzed top 10 countries by quantity sold
- Calculated top 10 countries by revenue
- Visualized all results using bar charts with Matplotlib

## Day 4 – Time-Based Sales Analysis

- Analyzed revenue patterns across different time frames
- Examined monthly revenue trends to identify high-performing months and seasonal patterns
- Analyzed revenue by day of the week to understand mid-week peaks and slower days
- Studied revenue by hour of the day and identified peak shopping hours (9 AM – 3 PM)
- Created month vs weekday sales heatmap to visualize daily and monthly revenue trends
- Documented key takeaways on peak hours, mid-week activity, late-year revenue spikes, top customers, and top products
- Noted anomalies and data caveats, such as partial December data

## Day 5 – RFM Customer Analysis

### Goal:
Analyze customer behavior using Recency, Frequency, and Monetary (RFM) metrics to identify active, loyal, and high-value customers.

### Steps:
- Built RFM table by CustomerID (Recency, Frequency, Monetary).
- Checked summary statistics for each metric.
- Visualized Recency distribution to identify active vs inactive customers.
- Visualized Frequency distribution to highlight occasional vs loyal buyers.
- Plotted Frequency vs Monetary scatter plot to spot high-value customers.

### Key Insights:
- Most customers are active but purchase only a few times.
- A small group buys frequently and spends more → loyal, high-value customers.
- Customers who haven’t purchased recently may need re-engagement campaigns.

### Takeaway:
Loyal, high-value customers drive most revenue and should be prioritized. Occasional buyers can be targeted with promotions to increase engagement.
