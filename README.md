# Sales-Analysis
[4:12 PM, 5/8/2026] M. Abdullah: https://jafri2022.gumroad.com/l/anspqu [7:06 PM, 5/8/2026] M. Abdullah: Executive-level Power BI Dashboard analyzing $34M+ sales data. Features advanced DAX for MoM growth tracking, dynamic field parameters for multi-metric analysis, and automated KPI monitoring for global confectionery operations.

 Executive Sales Intelligence Dashboard
📌 Project Overview
This project transforms raw transactional data from a global confectionery business into a high-impact executive dashboard. It provides a deep dive into $34.04M in total sales and $20.52M in profit, focusing on identifying growth trends and operational efficiencies.
🛠️ Technical Implementation (The "How")
I performed the following technical tasks to ensure the report is both scalable and insightful:
Advanced DAX Modeling: Developed complex measures for Month-over-Month (MoM) growth and performance indexing using CALCULATE, DATEADD, and VAR logic.
Dynamic Reporting: Implemented Field Parameters, allowing users to toggle the entire dashboard view between Sales, Profit, Cost, and Shipments dynamically.
Time Intelligence: Automated trend analysis to track performance fluctuations across a 12-month rolling window.
UX/UI Engineering: Designed Custom Report Tooltips and used Conditional Formatting to create a "Traffic Light" system (Good/At Risk) for shipment counts.
Geographic Insights: Segmented global market share, identifying the USA and India as primary revenue drivers (37%+ combined share).
🧠 DAX Showcase: MoM Sales Logic
MoM Sales Change % = 
VAR CurrentMonthSales = [Total Sales]
VAR PreviousMonthSales = CALCULATE([Total Sales], DATEADD('Date'[Date], -1, MONTH))
RETURN
DIVIDE(CurrentMonthSales - PreviousMonthSales, PreviousMonthSales)

Business Impact
Profit Audit: Identified that despite high volume, certain products required margin optimization to maintain the 60.3% average profit.
Operational Efficiency: The "Shipment Analysis" histogram pinpointed bottlenecks in the supply chain distribution.
