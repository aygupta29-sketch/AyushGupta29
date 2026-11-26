🛒 E-Commerce Store Analysis

An interactive Business Intelligence dashboard built with Microsoft Power BI to analyze e-commerce sales performance, customer purchasing behavior, product profitability, and regional sales trends.

The project turns raw transactional data into clear business insights through interactive visuals. This helps stakeholders track performance and make data-driven decisions.

Show Image Show Image Show Image

📑 Table of Contents
Project Overview
Business Objectives
Dashboard Preview
Key Performance Indicators
Dataset
Data Model
Dashboard Features
Key Business Insights
Tools & Technologies
Getting Started
Repository Structure
Future Improvements
Author
📌 Project Overview

E-commerce businesses generate large volumes of transactional data every day. Without proper analysis, it is difficult to spot sales trends, understand customer preferences, and find the most profitable product categories.

This dashboard gives a single, interactive view of business performance. It covers sales, profit, customer behavior, payment methods, and geographic trends.

🎯 Business Objectives

The dashboard answers key business questions such as:

Which states generate the highest sales?
Which customers contribute the most revenue?
Which product sub-categories generate the highest profit?
Which payment methods do customers prefer?
How does monthly profit change throughout the year?
Which product categories contribute the most to total quantity sold?
📊 Dashboard Preview
<p align="center"> <img src="dashboard_images/dashboard.png" width="100%" alt="E-Commerce Store Analysis Dashboard"> </p>
📈 Key Performance Indicators (KPIs)
KPI	Description
💰 Total Sales	Total revenue generated
📦 Total Quantity	Total number of products sold
💵 Total Profit	Overall business profit
🛍️ Average Order Value (AOV)	Average revenue per order (Total Sales ÷ Number of Orders)
📂 Dataset

The data is split into two CSV files:

File	Contents
Orders.csv	Order-level information: Order ID, Order Date, Customer Name, State, City
Details.csv	Line-item information: Order ID, Amount (Sales), Profit, Quantity, Category, Sub-Category, Payment Mode

Note: This dataset is used for learning and portfolio purposes only.

🔗 Data Model

The two tables are linked by Order ID in a one-to-many relationship:

text
Orders (1) ──── Order ID ────< (many) Details

One order in Orders can contain several products in Details.

Example DAX measures:

dax
Total Sales    = SUM(Details[Amount])
Total Profit   = SUM(Details[Profit])
Total Quantity = SUM(Details[Quantity])
AOV            = DIVIDE([Total Sales], DISTINCTCOUNT(Orders[Order ID]))
🧩 Dashboard Features
📌 Executive Overview
KPI cards for Total Sales, Total Profit, Total Quantity, and AOV
🌍 Regional Analysis
Sales by State
Orders by City (map visual)
💳 Payment Analysis
Quantity by Payment Mode
👥 Customer Analysis
Top Customers by Sales
📦 Product Analysis
Profit by Sub-Category
Quantity by Category
📅 Time Analysis
Monthly Profit Trend
Quarter slicer to filter the whole report
💡 Key Business Insights
Maharashtra recorded the highest sales of all states.
Clothing made up the largest share of total quantity sold.
Cash on Delivery (COD) was the most preferred payment method.
Printers generated the highest profit of all product sub-categories.
Monthly profit fluctuated noticeably, which suggests seasonal sales patterns.
A small group of customers contributed a large share of total revenue.
🛠️ Tools & Technologies
Tool	Purpose
Microsoft Power BI Desktop	Dashboard development
Power Query	Data cleaning and transformation
DAX	Measures and KPI calculations
SQL	Business queries on the raw data
CSV / Excel	Data source
📚 Skills Demonstrated
Data cleaning and transformation
Data modeling (relationships between tables)
DAX measures and KPI reporting
Interactive dashboard design
Data visualization and storytelling
SQL querying
Business analysis
🚀 Getting Started
Prerequisites
Microsoft Power BI Desktop (free, Windows only). Download it from the Microsoft Store or the Microsoft website.
Optional: a SQL database (MySQL, PostgreSQL, or SQLite) to run the queries in sql/.
1. Clone the repository
bash
git clone https://github.com/AyushGupta29/E-Commerce-Store-Analysis.git

Or click Code → Download ZIP on GitHub and extract it.

2. Open the dashboard
Open E-Commerce Store Analysis.pbix in Power BI Desktop.
Click Refresh to reload the data.
Use the slicers and click on visuals to cross-filter and explore.
3. Troubleshooting: "file not found" on refresh

The .pbix file stores the original location of the CSV files. If refresh fails:

Go to Home → Transform data → Data source settings.
Select each source and click Change Source.
Point it to your local dataset/Orders.csv and dataset/Details.csv.
Click Close & Apply, then Refresh.
4. Run the SQL queries (optional)
Import Orders.csv and Details.csv into your database as tables named Orders and Details.
Open sql/business_queries.sql and run the queries.
📁 Repository Structure
text
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
│   └── dashboard.png
│
└── sql/
    └── business_queries.sql
🔮 Future Improvements
Add year-over-year comparisons and a sales forecast
Add a customer segmentation page (for example, RFM analysis)
Add drill-through pages for state and product details
Publish the report to the Power BI Service for online viewing
👤 Author

Ayush Gupta GitHub: @AyushGupta29

⭐ If you found this project useful, please consider giving it a star!
