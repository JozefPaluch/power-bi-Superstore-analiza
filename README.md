# US Superstore Sales & Profitability Analysis

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-00599C?style=for-the-badge&logo=microsoft&logoColor=white)
![Power Query](https://img.shields.io/badge/Power_Query-7EAC41?style=for-the-badge&logo=microsoftexcel&logoColor=white)

## About the Project
This project focuses on analyzing the sales performance and profitability of a fictional "Superstore" in the United States. The goal was to build an interactive Power BI dashboard that uncovers time-based trends, geographical profit distribution, and key performance indicators, known as "KPI" to drive better business decisions.

## Key Business Insights
The analysis of the dataset revealed several actionable insights:
- Seasonality & Logistics: The highest sales peaks consistently occur in Q4 (the holiday season). This indicates a strong need to reinforce supply chain logistics and inventory levels during this period.
- Category Performance: The "Technology" category generates the highest net profit, despite not having the highest sales volume. Conversely, "Furniture" generates high revenue but suffers from the lowest profit margins.
- Regional Profitability: The West Region is the most profitable, driven largely by exceptional performance in California. However, several states in the Central Region operate at a loss, pointing to potentially flawed, overly aggressive discount policies.
- The Impact of Discounts: The data clearly shows that discounts exceeding 20% rarely translate into profit growth. While deep discounts significantly boost sales volume, they erode product margins too heavily to be financially viable.

## Technology Stack & Skills Demonstrated
- Power BI: Dashboard design and data visualization.
- Power Query: Data cleaning, type conversion, and handling regional currency settings.
- Data Modeling: Building a robust Star Schema (establishing active relationships between the Sales fact table and a dedicated Calendar dimension table).
- DAX language: Creating calculated measures for dynamic reporting.

## Key DAX Measures
```dax
Total Sales = SUM(superstore[Sales])
Total Profit = SUM(superstore[Profit])
Profit Margin = DIVIDE([Total Profit], [Total Sales], 0)
