🛒 E-Commerce Store Analysis
An interactive Business Intelligence Dashboard built using Microsoft Power BI to analyze e-commerce sales performance, customer purchasing behavior, product profitability, and regional sales trends.

This project transforms raw sales data into meaningful business insights through interactive visualizations, helping stakeholders monitor business performance and make data-driven decisions.

📌 Project Overview
E-commerce businesses generate large volumes of transactional data every day. Without proper analysis, identifying sales trends, customer preferences, and profitable product categories becomes challenging.

This dashboard provides a comprehensive overview of business performance by analyzing sales, profit, customer behavior, payment methods, and geographical trends through interactive visualizations.

🎯 Business Objectives
This dashboard helps answer key business questions such as:

Which states generate the highest sales?
Which customers contribute the most revenue?
Which product sub-categories generate the highest profit?
Which payment methods are most preferred?
How does monthly profit change throughout the year?
Which product categories contribute the most to total quantity sold?
📊 Dashboard Preview
E-Commerce Store Analysis Dashboard

🌍 Regional Sales Analysis
India E-Commerce Regional Sales Dashboard

💳 Payment & Customer Analysis
E-Commerce Payment and Customer Dashboard

📦 Product Performance Analysis
Product Performance Analysis Dashboard

📅 Time Analysis
Time Analysis - Monthly Profit Trend Dashboard

📈 Key Performance Indicators (KPIs)
KPI	Description
💰 Total Sales	Overall sales revenue generated
📦 Total Quantity	Total products sold
💵 Total Profit	Overall business profit
🛍️ Average Order Value (AOV)	Average revenue generated per order (Total Sales ÷ Number of Orders)
📂 Dataset Information
The dataset is split into two CSV files that are linked by Order ID:

File	Contents
Orders.csv	Order ID, Order Date, Customer Name, State, City
Details.csv	Order ID, Amount, Profit, Quantity, Category, Sub-Category, Payment Mode
Together, they include:

Customer Information
Product Categories
Sales Amount
Profit
Quantity
Payment Mode
State
City
Order Date
Note: This dataset is intended for learning and portfolio purposes only.

📊 Dashboard Features
📌 Executive Overview
Total Sales
Total Profit
Total Quantity Sold
Average Order Value (AOV)
🌍 Regional Analysis
Sales by State
Orders by City (Map Visualization)
💳 Payment Analysis
Quantity by Payment Mode
👥 Customer Analysis
Top Customers by Sales
📦 Product Analysis
Profit by Sub-Category
Quantity by Category
📅 Time Analysis
Monthly Profit Trend
Quarter-wise Filtering
🛠️ Tools & Technologies
Tool	Purpose
Microsoft Power BI	Dashboard Development
Power Query	Data Cleaning & Transformation
DAX	Measures & KPI Calculations
SQL	Business Queries & Data Validation
CSV / Excel	Data Source
📚 Skills Demonstrated
Data Cleaning
Data Transformation
Data Modeling
DAX Calculations
SQL Querying
KPI Reporting
Dashboard Development
Data Visualization
Business Intelligence
Business Analysis
Interactive Reporting
💡 Key Business Insights
Maharashtra recorded the highest sales among all states.
Clothing contributed the largest share of total quantity sold.
Cash on Delivery (COD) was the most preferred payment method.
Printers generated the highest profit among all product sub-categories.
Monthly profit showed noticeable fluctuations, indicating seasonal sales trends.
A small group of customers contributed a significant share of total revenue.
🚀 How to Use
Prerequisites
Microsoft Power BI Desktop (free, Windows only)
Optional: MySQL, PostgreSQL, or SQLite to run the SQL queries
Clone the Repository
git clone https://github.com/aygupta29-sketch/E-Commerce-Store-Analysis.git
Or click Code → Download ZIP on GitHub and extract it.

Open the Dashboard
Install Microsoft Power BI Desktop.
Open E-Commerce Store Analysis.pbix.
Refresh the data if required (see the note below).
Explore the dashboard using filters and slicers.
Note: If Refresh shows a “file not found” error, go to Home → Transform data → Data source settings, select each CSV source, click Change Source, and point it to dataset/Orders.csv and dataset/Details.csv on your computer. Then click Close & Apply.

Run the SQL Queries
Import Orders.csv and Details.csv into your database as tables.
Open sql/business_queries.sql.
Make sure the table names in the queries match the names you imported, then run them.
📁 Repository Structure
E-Commerce-Store-Analysis/
│
├── README.md
├── E-Commerce Store Analysis.pbix
│
├── dataset/
│   ├── Orders.csv
│   └── Details.csv
│
├── dashboard_images/
│   ├── dashboard.png
│   ├── India_E-Commerce_Sales_Dashboard.png
│   ├── E-Commerce_Payment_and_Customer_Dashboard.png
│   ├── product_analysis_dashboard.png
│   └── time_analysis_monthly_profit.png
│
└── sql/
    └── business_queries.sql
👤 Author
Ayush Gupta
GitHub: @aygupta29-sketch

⭐ If you found this project interesting, feel free to give it a star!
