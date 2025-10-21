📦 Operational Logistics & Supply Chain Performance Dashboard

Project Goal: To transform raw transactional data into a four-page strategic Power BI dashboard focused on cost reduction, velocity management, and supplier quality assessment, aligning with core business metrics.

Analyst: Stephen Chinenye Anyalewechi | 

www.linkedin.com/in/stephen-anyalewechi


🛠️ Technology Stack & Project Files

Report File: SUPPLY CHAIN POWER BI DASHBOARD.pbix

Source Data: supply_chain_data_cleaned.csv

Tools: Power BI Desktop (Power Query M, DAX), Data Visualization.

 Key Data Modeling & DAX Measures (Analyst Skills)

The foundation of this dashboard relies on creating meaningful, consolidated metrics. The table below details the core analytical formulas used:

| Metric Type | Example DAX Formula / Query Step | Purpose |
| :--- | :--- | :--- |
| **Cost Efficiency** | `Avg Cost per Product = DIVIDE(SUM([Shipping costs]), SUM([Number of products sold]))` | Benchmarks transportation expense directly to unit volume, allowing for effective carrier comparison. |
| **Velocity Metric** | `Avg Lead Time Days = AVERAGE([Lead time])` | Establishes the core measure of operational speed for the Executive Summary. |
| **Performance Value** | `Total Revenue from Slow Shipments = CALCULATE(SUM([Revenue generated]), [Lead time category] = "Slow")` | Quantifies the financial value tied up in underperforming logistics streams. |
| **Data Transformation** | Creation of a **`Lead time category`** column in Power Query | Segments continuous numerical data into actionable buckets (Fast, Medium, Slow) for visualization filtering. |

🚀 Key Insights & Dashboard Structure

The 4-page structure guides users from high-level financial impact to granular operational details:

1. Executive Summary & Performance Overview (The "What")

Focus: High-level financials and identifying immediate bottlenecks.

Core Visual: Volume vs. Speed Scatter Chart. This plots Total Products Sold (Volume) against Average Lead Time (Speed) to instantly highlight High-Volume/Slow-Fulfillment products (the "Bottlenecks") that require urgent operational intervention.

KPIs: Total Revenue, Total Profit, Total Products Sold, Total Profit Margin and Total Orders.

2. Logistics & Velocity Deep Dive (The "How Fast")

Focus: Identifying the most and least efficient components of the shipping process.

Key Scorecards:

Carrier Efficiency: Compares Avg Shipping costs against Avg Lead time to negotiate optimal contracts.

Transportation Mode Analysis: Breakdown of costs and speed by Road, Rail, and Air.

3. Inventory and Production Insights (The "How Prepared")

Focus: Managing quality risk and stock health.

Key Visuals: Supplier Defect Rate Scorecard (ranked by Avg Defect rates) to manage procurement risk, and analysis of manufacturing lead times against production volumes.

🌐 View and Interact

Download: Clone this repository to get the PBIX file.

Open: The report is self-contained. Open the SUPPLY CHAIN POWER BI DASHBOARD.pbix file in Power BI Desktop.

Explore: Navigate the four pages and interact with the slicers to see the analysis slice by different Routes and Product types.
