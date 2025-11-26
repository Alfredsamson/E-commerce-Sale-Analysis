E-Commerce Sales Analysis Project


Overview


This project performs a comprehensive analysis of e-commerce sales data from a fictional superstore, focusing on key metrics such as sales trends, profitability, customer segmentation, regional performance, and product categories. The analysis leverages pivot tables, dashboards, and raw datasets to uncover insights into sales performance across years (2014–2017), regions (Central, East, South, West), customer segments (Consumer, Corporate, Home Office), and more.
The project is built using Microsoft Excel for data processing, visualization, and reporting. It includes raw order data, pre-built pivot tables, and interactive dashboards to facilitate exploratory data analysis (EDA) and business intelligence (BI) tasks.



Key Insights from the Analysis



Total Sales: $2,297,200.86 across 9,994 orders from 793 unique customers.


Profitability: Overall profit of $286,397.02, with Technology products yielding the highest sales ($836,154.03) and Furniture showing variable profitability.


Top Performing Region: West region leads in sales ($725,457.82), while Central excels in efficiency (e.g., Indiana's $18,382.94 profit).


Customer Trends: Consumer segment drives the majority of sales ($1,161,401.34), with repeat customers like Sean Miller contributing significantly ($25,043.05).


Temporal Trends: Sales and quantity increased yearly, peaking in 2017 (12,476 units sold).


Returns: 297 orders were returned, highlighting potential areas for customer retention strategies.

Project Structure


The project uses two main Excel files:


1. Excel E-commerce Sales Project.xlsx



Sheet9: Simple state-level summary (e.g., Indiana and Grand Total rows—likely a partial pivot for quick reference).


Sheet2: Raw orders dataset (9,994 rows) with columns including:


Order details: Row ID, Order ID, Order Date, Ship Date, Delivery Duration, Ship Mode.


Customer info: Customer ID, Customer Name, Segment, Country, City, State, Postal Code, Region.


Product info: Product ID, Category, Sub-Category, Product Name.


Financials: Sales, Quantity, Discount, Discount Value, COGS, Profit.


Derived: Index, Modulo, Index.1.


Note: Data is truncated in the source; full dataset covers U.S.-based sales from 2014–2017.



Sheet1: Pivot table for profit by state (e.g., California: $76,381.39; Grand Total: $293,516.96).


Sheet3: Pivot table for customer count by state (e.g., California: 2,001; Grand Total: 7,055).


Sheet4: Pivot table for sales by segment (e.g., Consumer: $1,161,401.34; Grand Total: $2,297,200.86).


Sheet5: Pivot table for profit by year (e.g., 2017: $93,439.27; Grand Total: $286,397.02).


Sheet6: Pivot table for sales by top customers (e.g., Sean Miller: $25,043.05; Grand Total for sample: $88,281.80).


Sheet7: Dashboard title ("E-commerce DashBoard")—placeholder for visualizations.

2. pratical file.xlsx

Dashboard: High-level summary with key metrics:


Total Sales: $2,297,200.86.


Distinct Customers: 793.


Distinct Orders: 5,009.


Average Profit: $28.66.



Average Delivery Duration: 3.96 days.


Pivot Table: Multi-section pivot with:


Sales by segment (Consumer, Corporate, Home Office).


Sales by state (e.g., California: $457,687.63).


Quantity by year (e.g., 2017: 12,476).


Profit/Sales by sub-category (e.g., Phones: $330,007.05 sales, $44,515.73 profit).


Sales by region (e.g., West: $725,457.82).


Additional state and city breakdowns.

Sheet7: Empty sheet (potential for custom charts).


Orders: Full raw dataset (9,994 rows, similar to Sheet2 in the first file) with order-level details. Note: Heavily truncated in source; includes examples like high-value furniture orders.


People: Small lookup table for sample persons and regions (e.g., Anna Andreadi: West).


Shipping Cost: State-wise shipping costs per unit (e.g., Indiana: $2; Texas: $10).


Return: List of 297 returned orders by Order ID (e.g., CA-2017-153822).


Setup Instructions


Prerequisites:


Microsoft Excel (2016 or later) with PivotTable and Power Query support.


Installation:


Download the files: Excel E-commerce Sales Project.xlsx and pratical file.xlsx.


Open in Excel. Enable macros if prompted (though none are used here).


Refresh pivot tables: Select any pivot > Right-click > Refresh (Data > Refresh All).

Data Refresh:
Raw data in Orders sheets can be queried or filtered using Excel's built-in tools.


Use the Shipping Cost sheet to calculate total shipping expenses (e.g., via VLOOKUP or XLOOKUP).



Usage


Basic Analysis


Explore Raw Data: Open Sheet2 (first file) or Orders (second file). Filter by Region, Category, or Year (derived from Order Date).


View Pivots: Navigate to pivot sheets for quick summaries. Drag fields to slicers for interactivity.


Dashboard Interaction: In Dashboard sheet (second file), use slicers for segment/region filtering.

Advanced Steps

Calculate Shipping Totals: In Orders, add a column: =VLOOKUP(State, Shipping Cost!A:B, 2, FALSE) * Quantity.


Handle Returns: VLOOKUP Order ID against Return sheet to flag and subtract returns from profit calculations.


Visualizations:
Insert charts: Bar for sales by state, Line for yearly trends, Pie for category shares.
Example: In Pivot Table sheet, select data > Insert > Recommended Charts.v
