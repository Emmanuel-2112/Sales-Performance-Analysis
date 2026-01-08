# PROJECT
# 📊Sales-Performance-Analysis (Power BI Project)
# Company Overview
Eco Drive Motors is a UK-based automobile company selling Diesel, Petrol, and Electric vehicles to individual and fleet customers across multiple regions. The company aims to analyze two years of sales data using Power BI to understand sales trends, customer preferences, and environmental impact while aligning with sustainability goals and government regulations.
# Prepared By 
Taiwo Emmanuel 
# Project Date
December 2025
# Abstract
This project analyzes Eco Drive Motors’ vehicle sales data to evaluate business performance and sustainability impact in alignment with the UK government’s 2030 carbon reduction goals. Using Power BI, the project examines sales mix across Diesel, Petrol, and Electric vehicles, regional revenue contribution, customer acquisition and retention patterns, profitability by product line, and carbon emissions avoided through low-emission vehicle sales. Insights from this analysis provide actionable recommendations for optimizing sales strategy, improving profitability, and supporting the company’s transition toward environmentally sustainable mobility.
# Background
The automobile industry is shifting toward electric vehicles to reduce carbon emissions. In the UK, transport accounts for about 25% of CO₂ emissions, prompting a ban on new petrol and diesel cars by 2030 and a net-zero target by 2050. While EVs offer zero tailpipe emissions, challenges remain around adoption, infrastructure, and customer acceptance
# Project Statement 
Eco Drive Motors seeks to evaluate its overall business performance while measuring the environmental impact of its vehicle sales in line with the UK government’s 2030 carbon reduction targets. The project focuses on analyzing sales, revenue distribution, customer behavior, profitability, and carbon footprint reduction using Power BI, enabling data-driven decisions that support both commercial growth and sustainability goals
# Challenges
The following are challenges this project aims to solve:
- **Profitability vs Sustainability Trade-off:** Identifying vehicle types that support carbon-reduction goals while still delivering strong financial performance.
- **Uneven Regional Performance:** Understanding which regions drive revenue and which require targeted improvement strategies.
- **Profitability Assessment with Limited Cost Data:** Evaluating product-line profitability using maintenance cost as a practical proxy where full cost data is unavailable
# Project Objectives
The objective of this study is to;
- Analyze sales mix by vehicle type to identify adoption trends and shifts toward low-emission vehicles
- Assess customer acquisition and retention patterns, including repeat purchases and growth trends
- Estimate carbon footprint reduction achieved through EV and Hybrid sales in relation to 2030 targets
- Measure profitability by product line using gross profit and contribution margin analysis
-----
# DATA DESCRIPTION
# Data Source
The dataset originates from a consolidated sales and product management system designed to support sustainability-focused automotive operations. It integrates sales transactions, vehicle technology classifications, and regional customer data to enable performance evaluation aligned with environmental and regulatory objectives.
# Data Size and Format
The data is stored in Excel workbook format (.xlsx) and comprises multiple interrelated tables representing transactional sales data, product attributes, and customer location information. The dataset is of moderate size, allowing efficient transformation, modelling, and visualisation within Power BI.
# Calculated Columns
- Primary columns used in the analysis include: order id and order date, customer name and, location, vehicle model and vehicle type, units sold, selling price per unit, maintenance cost
- Key analytical measures created include: total revenue by vehicle type and region, contribution margin
# Data Collection
Data was compiled from simulated dealership sales records and product catalogue. Sales transactions were captured at the point of sale, while vehicle attributes such as type and maintenance cost were maintained centrally to ensure consistency across the organization.
# Data Characteristics
The dataset is:
- Clean and structured, requiring minimal pre - processing
- Well-suited for KPI - based analysis
- Environmentally contextual, enabling carbon impact evaluation
- Analytically robust, supporting both financial and sustainability reporting
------
# TOOLS USED
- **Microsoft Excel:** Served as the primary data source format, enabling structured storage of sales, product, and customer information.
- **Microsoft Power BI Desktop:** Used as the main analytics and visualization platform for KPI tracking, sustainability reporting, and performance assessment aligned with UK 2030 carbon reduction goals.
- **Power Query Editor:** Used for data cleaning, relationship preparation, and transformation processes to ensure analytical accuracy.
-----------------------
# METHODOLOGY 
# 1. Data Cleaning & Transformation
- Removed duplicate customer entries via dimensional modelling
- Normalized vehicle type values (Electric, Hybrid, Petrol)
- Filtered incomplete records
- Created dimension tables for Customers and Products
- Ensured maintenance cost consistency across product records
# 2. Data Modelling
- **a. Fact Table:** Order Details — transactional sales data at order level
- **b. Dimension Tables:** Product (Vehicle Type, Maintenance Cost), Customer (Location-based segmentation)
- **c. Relationship Design:** A star schema was implemented to enable cross-filtering between sales, customers, and vehicle types.
# 3. KPI Definitions
- **a. Sales Mix by Vehicle Type:** Analyses distribution of sales volume and revenue across Electric, Hybrid, and Petrol vehicles to identify shifts toward cleaner technologies.
- **b. Revenue Contribution by Region** Evaluates geographic revenue concentration to identify high-performing and underperforming regions.
- **c. Customer Acquisition & Retention** Assesses repeat purchase behaviour to understand customer loyalty and growth patterns.
- **d. Carbon Footprint Reduction:** Estimates emissions avoided through low-emission vehicle sales, supporting UK 2030 sustainability targets.
- **e. Profitability by Product Line:** Uses contribution margin (Revenue − Maintenance Cost) to compare financial performance across vehicle types.
# 4. DAX Measures
## Total Revenue 
```DAX
Total Revenue =
SUMX( 'Order Details','Order Details'[Units Sold]*'Order Details'[Selling Price Per Unit (£)])
```

- Full DAX Measures and DAX Columns below
[ECODRIVE  DAX MEASURE.pdf](https://github.com/user-attachments/files/24492416/ECODRIVE.DAX.MEASURE.pdf)

-----
# EXPLORATORY DATA ANALYSIS (EDA)
# Dashboard
# Page 1: Sustainability & Market Performance
- Visual 1: Vehicle Sales Distribution (Donut Chart)
  - Purpose: Highlights adoption of low-emission vehicles relative to petrol cars.
  - KPIs linked: Sales Mix by Vehicle Type

- Visual 2: Revenue by Region (Bar Chart)
  - Purpose: Shows geographic revenue concentration.
  - KPIs linked: Revenue Contribution by Region

# Page 2: Customer & Profit Insights
  - Visual 3: Customer Retention Analysis (Column Chart)
    - Purpose: Evaluates repeat purchase behaviour.
    - KPIs linked: Customer Acquisition & Retention

- Visual 4: Profitability by Vehicle Type (Bar Chart)
  - Purpose: Compares contribution margins across vehicle categories.
  - KPIs linked: Profitability by Product Line

## Dashboard–Insight Traceability Table

# Key Findings
- Sales Mix analysis shows increasing adoption of low-emission vehicles, particularly Electric and Hybrid models.
- Regional Revenue Contribution varies significantly, indicating opportunities for geographic optimization.
- Repeat Customers demonstrate higher engagement and revenue contribution than new customers.
- Carbon Footprint Reduction Metrics confirm meaningful progress toward long-term emission reduction targets.
- Contribution Margin analysis highlights Electric vehicles as more financially sustainable despite higher operational costs.

# Rationale
- Sales Mix on each of the vehicle type helps to understanding customer demand patterns and product portfolio performance
- Revenue Contribution By Region highlights geographical performance differences and identifies where the business is thriving or underperforming
- Customer Acquisition and Retention Analysis helps Eco Drive Motors understand buying behaviour, loyalty, and long term revenue sustainability.
- Carbon Footprint Reduction evaluates Eco Drive Motors’ contribution to environmental sustainability by estimating emissions avoided through Electric and Hybrid vehicle sales.
- Profitability By Product Line evaluates how much each vehicle type contributes to the company’s financial performance after accounting for variable costs. 

# Recommendations
- Accelerate Electric vehicle adoption to strengthen regulatory compliance and sustainability credentials.
- Reallocate resources toward high-performing regions while implementing corrective strategies in lagging areas.
- Strengthen customer retention initiatives to maximise lifetime value.
- Use contribution margin insights to refine pricing and product strategy.

# Conclusion
The EcoDrive Motors dashboard demonstrates how integrated analytics can support environmentally responsible decision-making while maintaining strong financial performance
