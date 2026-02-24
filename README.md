# Customer-Churn-Exit-Rate-Analysis-Power-BI
🔹**Project Overview**
Designed an end-to-end Power BI customer churn analytics dashboard to identify churn patterns, exit risk drivers, and retention opportunities across multiple customer dimensions. The dashboard enables stakeholders to quickly understand who is leaving, why they are leaving, and where intervention is required.

**🔹Business Problem**
The bank was experiencing increasing customer attrition but lacked visibility into:
Exit trends over time
High-risk customer segments
Impact of credit score, card ownership, and demographics on churn
The goal was to convert raw customer data into actionable insights for retention strategy planning.

**🔹Dataset**
Source: Simulated Banking Customer Churn Dataset
Records: 10,000+ customer records
Time Period: 2016–2019

**Key fields included:**
Customer ID, Age, Gender, Geography
Credit Score, Credit Rating
Card Holder Status
Active / Inactive Status
Exit Indicator

**🔹 Tools & Technologies Used**
Power BI Desktop – Data modeling, DAX, visualization
Power Query – Data cleaning & transformation
DAX – Measures for KPIs and Exit Rate calculations

**🔹 Data Preparation & Modeling**
Cleaned and standardized raw data using Power Query
Created derived columns (Active Status, Credit Rating categories)

**Built a star schema data model with:**
Fact table: Bank_Churn
Dimension tables: Gender, Geography, Credit Card, Exit Customer
Established one-to-many relationships to enable accurate slicing

**🔹 Key KPIs Created (DAX)**
Total Customers
Active vs Inactive Customers
Exited Customers
Retained Customers
Credit Card Holders vs Non-Holders

**Exit Rate %**
Example:
Exit Rate % = 
DIVIDE(
    CALCULATE(COUNT(CustomerId), Exited = 1),
    COUNT(CustomerId)
)

**🔹 Key Visual Insights**
📈 Exited Customers by Year – Identified increasing churn trend over time
📊 Exit Rate % by Year – Normalized churn for fair year-to-year comparison
👩‍🦰👨 Exited Customers by Gender – Gender-based churn comparison
💳 Exited Customers by Card Holder Status – Higher exits among card holders (needs rate analysis)
📉 Exited Customers by Credit Rating – Poor credit score customers show significantly higher churn

**🔹 Business Insights**
Customers with poor credit ratings are at the highest churn risk
Exit rate peaked around 2017–2018, indicating process or policy impact
Card holders show higher churn count, highlighting need for rate-based evaluation
Gender-based churn differences suggest targeted retention campaigns

**🔹 Recommendations**
Introduce early-warning churn alerts for low credit score customers
Redesign credit card benefits to improve engagement
Focus retention programs during high-risk years identified by exit rate
Use exit rate (not just counts) for strategic decision-making

**🔹 What This Project Demonstrates**
Strong understanding of business problem framing
Ability to design clean data models
Practical use of DAX measures vs calculated columns
Analyst mindset: moving from counts → rates → insights
