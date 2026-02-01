# Healthcare-Claims Tracker
Healthcare Claims & Cost Variance Tracker (In-Progress)
📊 Project Overview
This Power BI dashboard was developed to provide an executive-level overview of a healthcare claims dataset totaling $23M. The goal of the project is to identify financial trends, analyze denial rates, and pinpoint high-cost provider specialties to assist in Claims Integrity and Revenue Cycle Management.

🛠️ Key Features & Insights
Executive KPI Header: Real-time tracking of Total Claims ($23M), Average Claim Cost ($5.01K), and a high-level Denial Rate (34%).

Cost Variance Analysis: A time-series line chart tracking spend from 2022 to 2024, identifying a significant peak in 2023 ($11.8M) followed by a sharp decline.

Root Cause Denial Table: A specialized table using Conditional Formatting (Heat Map) to highlight specialties with denial rates exceeding 30%, specifically targeting Orthopedics and Pediatrics.

Demographic Segmentation: Analysis of spend across Patient Gender (50.77% Female vs 49.23% Male) and Employment Status to identify primary cost drivers.

Interactive Discovery: Integrated slicers for Year, Month, Provider Specialty, and Location to allow for granular data filtering.

🧠 Technical Skills Applied
Data Modeling: Established a Star Schema to connect claim facts with a centralized Calendar Table for accurate time-intelligence reporting.

DAX (Data Analysis Expressions):

Total Claims $ = SUM(Table[ClaimAmount])

Denial Rate % = DIVIDE( CALCULATE(COUNT(ID), Status="Denied"), COUNT(ID) )

Calculated measures for Average Claim Cost to standardize unit economics.

Data Visualization: Utilized Clustered Bar Charts, Donut Charts, and advanced conditional formatting to improve "Time-to-Insight" for auditors.

Data Cleaning: Handled data type conversions (Text to Decimal) to ensure mathematical accuracy of currency values.

📈 Business Impact
By using this dashboard, a Claims Integrity team can:

Prioritize Audits: Focus on the "General Practice" specialty which currently holds a 35% denial rate.

Budget Forecast: Use the 2023 spend peak to predict future seasonal surges.

Operational Efficiency: Identify that "Paper" and "Phone" claim submissions (visible in the detail table) may be contributing to higher processing costs compared to "Online" submissions.
