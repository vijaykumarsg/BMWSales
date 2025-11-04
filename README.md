1. Project Overview
The Car Sales Analytics Dashboard is a Power BI project designed to analyze and visualize car sales data across multiple brands, models, and regions.
The goal of this project is to transform raw sales data into actionable business insights that help stakeholders track performance, identify trends, and make data-driven decisions.

2. Objectives
   1.Analyze total car sales and revenue distribution across various brands and models.
   2.Identify top-performing and underperforming car categories.
   3.Provide insights into sales patterns by region, time period, and price segment.
   4.Enable management to monitor key performance indicators (KPIs) such as total sales, revenue growth, and average selling price.

3. Data Description
  Dataset Components:
  Brand: Car brand name (e.g., Toyota, BMW, Hyundai, etc.)
  Model: Car model name
  Region: Geographic area of sales
  Units Sold: Number of cars sold
  Revenue: Total revenue generated per brand/model
  Price: Average price per unit
  Date: Sales date or month
  Data Source:
  Data imported from Excel (or CSV).
  Cleaned and transformed using Power Query in Power BI.

4. Data Cleaning & Transformation
  Performed in Power Query Editor:
  Removed nulls, duplicates, and inconsistent entries.
  Standardized column names and data formats (e.g., date, currency).
  Created calculated columns for:
  Revenue per unit
  Profit margin
  Sales growth %
  Built data relationships between different tables (if applicable).

5. Dashboard Design
  The dashboard was structured into three key pages/views:
  Page 1: Sales Overview
    KPIs: Total Sales, Total Revenue, Average Price, YoY Growth
    Visuals: Line chart (monthly trend), bar chart (brand performance), card visuals
  Page 2: Brand & Model Analysis
    Brand vs Model-wise performance breakdown
    Market share visualization (donut/pie chart)
    Top 5 and bottom 5 models by sales
  Page 3: Regional Insights
    Map visualization for region-wise sales
    Comparative analysis of region-wise demand
    Filters for region, brand, and year

6. DAX Measures Used
    Total Sales = SUM(Sales[Units Sold])
    Total Revenue = SUM(Sales[Revenue])
    Average Price = AVERAGE(Sales[Price])
    YoY Growth = (Current Year Sales - Previous Year Sales) / Previous Year Sales
    Top Brands = RANKX(ALL(Sales[Brand]), [Total Revenue])
    These DAX measures help generate KPIs and enable dynamic filtering for real-time analysis.

7. Key Insights
    Identified top 3 brands contributing over 60% of total revenue.
    Region A shows highest growth rate compared to others.
    Average price impacts total revenue more strongly than volume in some segments.
    Visual insights enabled management to plan inventory and marketing more efficiently.

8. Business Impact
    Improved sales visibility across multiple dimensions (brand, region, time).
    Enabled faster decision-making with real-time Power BI dashboards.
    Supported data-driven sales strategy through trend and performance analytics.

9. Tools & Technologies
    Category	Tools Used
    Data Visualization	Power BI
    Data Preparation	Power Query
    Data Modeling	DAX, Relationships
    Source Data	Excel / CSV
    Documentation	PowerPoint, Markdown

10. Author
    Vijay Kumar S G
    viji03662@gmail.com

11. Future Enhancements
    Integrate live data sources (SQL or API).
    Add predictive insights using Python or Power BI Forecasting.
    Include Customer Satisfaction & Service data for holistic analytics.

