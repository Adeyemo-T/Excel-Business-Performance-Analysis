# Excel-Business-Performance-Analysis
.l# Business Performance Dashboard: Tracking Revenue and Customer Insights

## Project Background

A retail or e-commerce business requires a holistic dashboard solution to continuously monitor key operational health metrics, track YOY performance changes, and identify high-value customer segments. The goal is to provide a single source of truth for Sales, Supply Chain (Quantity), and Marketing (Customer Insight).

This project delivers a complete overview of commercial performance, focusing on YOY variance to reveal growth drivers and potential bottlenecks.

Insights and recommendations are provided on the following key areas:
* **YOY Performance Tracking:** Analysis of year-over-year growth in Revenue, Quantity, and Average Unit Price.
* **Customer Segmentation:** Identification of the highest value customer groups and trends in customer retention.
* **Supply Chain Optimization:** Evaluation of the top-selling product units (OZ, CT, CANS) to inform inventory and stocking decisions.
* **Geographical Distribution:** Mapping of sales performance across global regions to guide marketing and logistics allocation.



* **Interactive Dashboard:** The full Business Performance dashboard can be accessed [here](LINK_TO_POWER_BI_DASHBOARD).
* **Analysis Code:** The underlying Excel files and pivot table calculations can be found [here](LINK_TO_CODE_FILE).

## Data Structure & Initial Checks

#### Data Overview
The analysis was built on a **Star Schema** data model created in Power Pivot/Power BI, linking multiple dimensions to a central fact table. The data was sourced from **multiple separate Excel files** (including Transaction, Product, Supplier, and Customer files) to ensure a comprehensive view of the business.

#### 🔗 Data Model (Star Schema)
The model consists of a central **Fact Table** (containing metrics like `Total Sales`, `Quantity`, and `Unit Price`) linked to several **Dimension Tables** (e.g., `item_dim`, `time_dim`, `customer_dim`, `store_dim`).


*(**Action:** Insert the image of your **Power Pivot/Excel Data Model View** showing the connected tables.)*

#### Data Cleaning and Preparation
The data cleaning and preparation process was executed using a combination of **Excel functionality** and **Power Query (M Language)**, which is essential for transforming raw transactional data into a Star Schema structure.

* **ETL (Extract, Transform, Load) with Power Query:** Power Query was used to merge, append, and shape the raw data files, handle data typing, and ensure unique keys were present in all dimension tables.
* **Metric Aggregation (Excel Pivot Tables):** **Pivot Tables** were used extensively in Excel to summarize and calculate the core business metrics shown on the dashboard, such as **YOY % changes** for Revenue, Quantity, and Average Unit Price.
* **Custom Calculations:** YOY calculations (`Revenue YOY`, `Quantity YOY`) were derived directly from the underlying data model to provide the immediate comparative insights shown on the KPIs.

## Executive Summary

The business shows a healthy upward trend with total **Revenue reaching $30M** and positive **Year-over-Year (YOY) growth in Revenue (2.18%)** and **Quantity (2.13%)**. However, the long-term viability is threatened by a high concentration of revenue—**90% of transactions are conducted via mobile**, and a significant portion of sales relies on just **three customers**. Strategic focus must immediately pivot to diversifying transaction types, stabilizing the monthly sales volatility, and addressing the poor performance in key supplier relationships.

#### Overview of Operational Health

* **Positive YOY Growth:** The company achieved strong YOY growth in both **Revenue (2.18%)** and **Quantity Sold (2.13%)**, demonstrating successful expansion across its markets.
* **Customer Concentration Risk:** Customer Insight analysis shows sales are heavily dependent on a few key individuals (e.g., Jyoti, Pooja), indicating a **high retention risk** if any of these top customers are lost.
* **Transaction Bottleneck:** A staggering **90% of transactions occur via mobile**, creating a single point of failure and potential bottleneck in the payment infrastructure.

![Overall KPIs and Customer Insight](YOUR_IMAGE_LINK_FOR_KPI_AND_CUSTOMER_INSIGHT_CHART_HERE)
*(**Action:** Insert the image link showing the **Revenue KPI, Quantity KPI, Average Unit Price KPI, Transaction Type chart, and Customer Insight chart**.)*

#### Supplier & Product Performance

* **Top Products:** The top-selling categories are **Beverage/Energy/Protein** and **Healthy Foods**, indicating strong market demand for health and wellness products.
* **Supplier Disparity:** The **Top 10 Suppliers** show large variance in their contribution, confirming the need to optimize procurement based on performance and reliability.
* **Logistics Focus:** The primary unit of sale is **'oz' (128K units)**, followed by **'ct' (659K units)**, which is critical information for warehouse stocking and logistics teams.

![Top Selling Products and Supplier Performance](YOUR_IMAGE_LINK_FOR_PRODUCTS_AND_SUPPLIERS_CHART_HERE)
*(**Action:** Insert the image link showing the **Top Selling Products** bar chart and the **Supplier Performance** chart.)*

#### Geographical & Divisional Performance

* **Global Distribution:** Sales are concentrated in **Bangladesh, Germany, and India**, which should guide marketing budget allocation.
* **Domestic Disparity:** The map and bar chart show significant sales disparity across domestic divisions (e.g., Sylhet, Rangpur, Dhaka), confirming that resource allocation should be prioritized toward the highest-performing districts.
* **Week-Over-Week Trend:** The weekly trend shows a strong surge in sales during the **4th week**, suggesting targeted promotional activities may be most effective near the end of the month.

![Geographical Map and Divisional Performance](YOUR_IMAGE_LINK_FOR_MAP_AND_DIVISIONS_CHART_HERE)
*(**Action:** Insert the image link showing the **Global Map, Divisional Performance chart, and Week Trend chart**.)*

## Business Recommendations

Based on the analysis of YOY metrics, customer insights, and distribution performance, the following actions are critical to diversify risk and maximize future revenue growth:

* **1. Mitigate Customer Concentration Risk:** Immediately implement a strategy to **reduce reliance on the top three customers** (Jyoti, Pooja, etc.). This involves enhancing the loyalty program for the next tier of customers and focusing marketing efforts on acquisition to stabilize the customer base.
* **2. Diversify Payment Channels:** The **90% dependency on mobile transactions** presents a single point of failure. Investigate the low adoption of Card and Cash transactions and implement incentives to encourage the use of alternative payment methods.
* **3. Optimize Supplier Relationships:** Conduct a thorough performance review of all top suppliers. Prioritize procurement contracts with the most efficient partners to ensure stable inventory and cost control.
* **4. Targeted Divisional Investment:** Use the geographical data to **prioritize resource allocation** in the highest-performing divisions (e.g., Sylhet, Rangpur). Invest in targeted marketing and optimized logistics to maximize returns in these proven markets.
* **5. Align Promotion with Week Trend:** Leverage the strong sales surge observed in the **4th week** of the month. Strategically schedule product promotions and marketing pushes to coincide with this peak purchasing period to maximize revenue impact.

---

Thank you for reading! Leave a comment if you have any questions about the analysis.
