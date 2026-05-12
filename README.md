📊 SuperStore Sales Analysis & Dashboard
An end-to-end retail sales analytics project analyzing 5,900+ transactions across 2019–2020 — from raw data transformation to interactive dashboards and a 15-day sales forecast — built entirely in Microsoft Power BI.

📌 Overview
Problem Statement:

"How can a retail business leverage historical sales data to identify revenue drivers, uncover profit gaps, and anticipate future demand?"

This project covers a complete analytics pipeline using Power BI as the sole platform:

Cleaning and transforming raw data with Power Query
Building KPIs and calculated metrics using DAX
Designing 4 interactive dashboards for business insights
Forecasting the next 15 days of sales using Power BI's built-in ETS model


📂 Dataset
AttributeDetailSourceSuperStore Sales Dataset (CSV)Records5,901 rowsUnique Orders3,003Unique Customers773PeriodJanuary 2019 – December 2020Features23 columns
Feature Groups:
GroupColumnsOrder Infoorder_id, order_date, ship_date, ship_modeGeographyregion, state, cityCustomercustomer_name, segmentProductcategory, sub_category, product_nameFinancialssales, profit, quantityPaymentpayment_mode

🛠️ Tools & Technologies
ToolPurposePower Query (M Language)Data cleaning, transformation & normalizationDAX (Data Analysis Expressions)KPIs, measures & calculated columnsPower BI Report CanvasInteractive dashboards & visualizationsPower BI Analytics Pane15-day sales forecasting (ETS algorithm)

🔄 Project Steps
1. 🔧 Data Transformation (Power Query)

Promoted headers and corrected data types across all 23 columns
Parsed Order Date and Ship Date to proper Date format
Derived a Delivery Days calculated column
Removed duplicates and handled null values
Normalized categorical fields (Region, Segment, Category)

2. 🗂️ Data Modeling

Built a star schema with a central Sales fact table
Linked dimension tables for Date, Product, Customer, and Geography
Enabled efficient cross-filtering across all dashboard visuals

3. 📐 DAX Measures
Key measures built using DAX:

Total Sales, Total Profit, Profit Margin %
YoY Sales Growth, Monthly Sales Trend
Average Delivery Days, Order Count

4. 📈 Power BI Dashboards
Four interactive report pages with dynamic slicers for Date, Region, Segment, and Category.
PageContentSales OverviewKPI cards, monthly trend line, regional revenue mapCategory & ProductRevenue vs. profit by category, sub-category treemapCustomer & SegmentSegment split, payment mode, shipping preference, top customersGeographic MapChoropleth map by state, city-level bubble drill-down
5. 🔮 Sales Forecasting

Applied Power BI's built-in forecasting on the daily sales time series
Horizon: 15 days beyond December 31, 2020
Algorithm: Exponential Smoothing (ETS)
Confidence Interval: 95%
Forecast signals continued elevated demand consistent with Q4 seasonality


🔍 Key Results

$1.57M total revenue · $175K net profit · 11.2% overall margin
Technology is the most profitable category at 19.2% margin
Furniture generates $451K in revenue but only a 2.2% margin — needs review
West region leads with 33.4% of total sales, driven by California ($335K)
Consumer segment contributes 48% of revenue
COD is the dominant payment method at 42.6% — a cash-flow risk
Standard Class shipping handles 58% of all orders
15-day forecast projects sustained high daily sales into early January 2021


🚀 How to Run
Prerequisites

Power BI Desktop (free) — Download here

Steps
1. Clone the repository
bashgit clone https://github.com/your-username/superstore-sales-powerbi.git
cd superstore-sales-powerbi
2. Open the Dashboard

Launch Power BI Desktop
Open SuperStore_Sales_Dashboard.pbix
If prompted, update the data source path to point to data/SuperStore_Sales_Dataset.csv
Click Refresh to reload the data

3. Explore

Use the slicers (Region, Segment, Category, Date) to filter across all visuals
Navigate to the Sales Overview page and open the Analytics pane to view the 15-day forecast


📁 Project Structure
superstore-sales-powerbi/
│
├── data/
│   └── SuperStore_Sales_Dataset.csv      # Raw dataset
│
├── dashboard/
│   └── SuperStore_Sales_Dashboard.pbix   # Power BI dashboard file
│
├── report/
│   └── SuperStore_Sales_Project_Report.pdf
│
└── README.md

👤 Author
Shubham

Built entirely with Microsoft Powerbi
LinkedIn · GitHub

Built entirely with Microsoft Power BI
