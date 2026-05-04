

# HDI PCB Manufacturing Dashboard (Power BI)

This project builds on the SQL-based root cause analysis and transforms manufacturing data into a dashboard for monitoring yield, defects, scrap, rework, and process performance.

The goal is to support real-time decision-making in manufacturing operations.
This project presents a **manufacturing KPI dashboard** built in Power BI to monitor **quality, yield, and operational performance**.  
An HDI PCB production scenario is used as a **high-complexity example**, while the dashboard design and analytical logic are **transferable to other manufacturing environments**.
## Relationship with SQL Project

This dashboard is built on the SQL-based root cause analysis:

👉 https://github.com/KarimTheAnalyst/HDI-PCB-Root-Cause-SQL

- SQL is used to structure data, calculate KPIs, and identify patterns
- Power BI is used to visualize performance and support decision-making

## Dashboard Pages

1. **Executive Summary (Manufacturing Performance Overview):**  
   High-level monitoring of key manufacturing KPIs, including yield, defect rate, scrap, rework, and overall process performance.

2. **Quality & Root Cause Analysis:**  
   Detailed analysis of defect distribution, scrap rates, and root cause drivers across machines, materials, and product characteristics.

3. **Operational Efficiency:**  
   Analysis of machine performance, downtime, and maintenance activities, including maintenance cost and breakdown patterns.

---

## Data Source

This project uses a synthetic dataset designed to simulate a realistic HDI PCB manufacturing environment.

The dataset was structured to reflect key aspects of production, including yield, defects, scrap, rework, maintenance, and process variability.

While the data is simulated, the data model, DAX measures, and analytical approach are aligned with real-world manufacturing analytics practices and support realistic business scenarios.
---

##  Dashboard showcase

### **Page 1: Executive Summary (Manufacturing Performance Overview)**  
*Provides a high-level view of manufacturing performance and key operational KPIs.*

![Executive Summary](https://private-us-east-1.manuscdn.com/sessionFile/OZ9GS0NtDjJ0n2OGiayvZE/sandbox/jxMN45Q1cOFlXZ93eSlimq-images_1764425186934_na1fn_L2hvbWUvdWJ1bnR1L3BhZ2UxX2V4ZWN1dGl2ZV9zdW1tYXJ5.png?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9wcml2YXRlLXVzLWVhc3QtMS5tYW51c2Nkbi5jb20vc2Vzc2lvbkZpbGUvT1o5R1MwTnREakowbjJPR2lheXZaRS9zYW5kYm94L2p4TU40NVExY09GbFhaOTNlU2xpbXEtaW1hZ2VzXzE3NjQ0MjUxODY5MzRfbmExZm5fTDJodmJXVXZkV0oxYm5SMUwzQmhaMlV4WDJWNFpXTjFkR2wyWlY5emRXMXRZWEo1LnBuZyIsIkNvbmRpdGlvbiI6eyJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTc5ODc2MTYwMH19fV19&Key-Pair-Id=K2HSFNDJXOU9YS&Signature=UO6wpvao6VVUYyo2UO~o6AU6PSxUf5Lug~GEUMWptsJi04w3mmEGvp2Eyfvm318~YuHfTm9DmYAEVc49JcTZLIOqen~gcKPxDHRHP~--SqbAnSdLaZ95~Y-PWSSujFQQ~JrLrpCc6wWvmHhe6KrWLdd12SBfQEgNN0g50Vvs5NcSxNxwTZq5g5P25Te0RFD2jK1HOcrfqvSZIjJK3t7dCx9ehPVNnitxKeTVgYDt~eswG8GrppFLheoezrDMNLHQO68wavT0SgIXAU8A7GF~wcVztqxzPG0a7J2qMj5GsBBb36ckr1wc1ZF4KtXAQHn1Te5xb7ZVXJR-eMWq~km39A__)

**Insights:**
- Overall yield and defect trends provide a quick view of production performance
- Scrap and rework rates highlight the impact of quality issues on operations
- Performance trends over time help detect process instability or improvement
- KPI monitoring supports early identification of production risks
---

### **Page 2: Quality & Root Cause Analysis**  
*Identifies key drivers of defects, scrap, and quality variation across materials, machines, and product characteristics.*

![Quality & Root Cause Analysis](https://private-us-east-1.manuscdn.com/sessionFile/OZ9GS0NtDjJ0n2OGiayvZE/sandbox/jxMN45Q1cOFlXZ93eSlimq-images_1764425186937_na1fn_L2hvbWUvdWJ1bnR1L3BhZ2UyX3F1YWxpdHlfYW5hbHlzaXM.png?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9wcml2YXRlLXVzLWVhc3QtMS5tYW51c2Nkbi5jb20vc2Vzc2lvbkZpbGUvT1o5R1MwTnREakowbjJPR2lheXZaRS9zYW5kYm94L2p4TU40NVExY09GbFhaOTNlU2xpbXEtaW1hZ2VzXzE3NjQ0MjUxODY5MzdfbmExZm5fTDJodmJXVXZkV0oxYm5SMUwzQmhaMlV5WDNGMVlXeHBkSGxmWVc1aGJIbHphWE0ucG5nIiwiQ29uZGl0aW9uIjp7IkRhdGVMZXNzVGhhbiI6eyJBV1M6RXBvY2hUaW1lIjoxNzk4NzYxNjAwfX19XX0_&Key-Pair-Id=K2HSFNDJXOU9YS&Signature=TyDKgUXBBOhfc-6BrtFwFUT9qhDx2n08vZGGTsJFISP3QLS6VgEYwwgr0PclYdhTcb-5SUeC3n7mY94kq6oDRRe2Tu1uWWx--vWptCQxuFm-UYrYIzDvlYEHFr1mDgBHCl4ndJbmIdsdhS~h73V-6PxIjse3Ol2Uv3hL-CC9sz7P-LU5SjorggLMSw~2Mnp0jtzQpgWxy2Ay-cIC08x1Z~6yNQlljomnp6ppkFpURjVgcgPOl74eX7Krov3BZKycSR3DKt9F9QOaTzD0rRpX7BLFU2ckJDYBzZG5Cj-DSxit6sV562p7HrmZTrv7Kr2cb6kKW9vJ8mWcwv6CC60CzQ__)

**Insights:**
- Overall scrap rate of 4.45% across 1,000 production orders highlights measurable quality loss
- Megtron 6 material shows the highest scrap rate (4.84%), suggesting higher process sensitivity or material-related issues
- Short circuits are the primary defect mechanism (150 occurrences), followed by delamination and contamination
- Scrap rate improved from 8% in Q1 2023 to 2% in Q4 2025, indicating improved process control and quality performance

**Interpretation:**
- Defect concentration points to specific process steps requiring investigation
- Material-related variation suggests the need for tighter process control or supplier evaluation
- Tracking defect trends over time supports continuous improvement initiatives
---
### **Page 3: Operational Efficiency & Maintenance**
*Evaluates machine performance, downtime, and maintenance activities to support reliability improvement and production stability.*

![Operational Efficiency](https://private-us-east-1.manuscdn.com/sessionFile/OZ9GS0NtDjJ0n2OGiayvZE/sandbox/jxMN45Q1cOFlXZ93eSlimq-images_1764425186938_na1fn_L2hvbWUvdWJ1bnR1L3BhZ2UzX29wZXJhdGlvbmFsX2VmZmljaWVuY3k.png?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9wcml2YXRlLXVzLWVhc3QtMS5tYW51c2Nkbi5jb20vc2Vzc2lvbkZpbGUvT1o5R1MwTnREakowbjJPR2lheXZaRS9zYW5kYm94L2p4TU40NVExY09GbFhaOTNlU2xpbXEtaW1hZ2VzXzE3NjQ0MjUxODY5MzhfbmExZm5fTDJodmJXVXZkV0oxYm5SMUwzQmhaMlV6WDI5d1pYSmhkR2x2Ym1Gc1gyVm1abWxqYVdWdVkzay5wbmciLCJDb25kaXRpb24iOnsiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE3OTg3NjE2MDB9fX1dfQ__&Key-Pair-Id=K2HSFNDJXOU9YS&Signature=OxmmIy0pZKl8PGNsxRErlErZmD-6lPIx7lAkmp9JvrVsPLr0r9c5XPjDLdhmw-VXWQc~LlUDZyGthw4rr1~SQXQ6PeuJEdiwbkA3q5sKqpT5Kw5b9QNxeC8wAHLZYS9w44pOMYTm5uaRNkpl4ppHdWgwGddnh7DTmdLr8Dm9UMdozSxmq6F1--1nxesE8v~cChqRnFiKBALLr30eypwuUOHg994TZfbfV58UOZFCLr5NpCrkhWxGqAQMxft9OLCrPoifbIzobpCZG-bA2WzPcWs~IyN6VfOAoM8LxtJdk8DXYepaEEs3Q7tjDAz2sV944YXJtlhP0~UWqHqk~Px0QQ__)

**Insights:**
- Total maintenance cost of $831K with 5.6K hours of downtime indicates a significant impact on production availability
- SM-1 machine has the highest maintenance cost ($39K), making it a priority candidate for detailed inspection or overhaul
- Preventive maintenance represents 60% of total events (519), reflecting a structured maintenance approach
- Breakdown rate of 39.9% (Emergency + Corrective) suggests opportunities to further shift toward preventive maintenance
- Maintenance cost shows quarterly variability, with peaks in Q4 2024 and Q4 2025, indicating potential periods of increased operational stress

**Interpretation:**
- High-cost machines should be prioritized for reliability analysis and preventive actions
- Reducing breakdown frequency can improve uptime and overall production stability
- Monitoring maintenance trends supports better planning and resource allocation
---
## Technical details

### Project Objectives

- Build an end-to-end manufacturing analytics dashboard for HDI PCB production
- Monitor key KPIs including yield, defects, scrap, rework, and maintenance performance
- Support root cause analysis and process improvement decisions
- Provide clear visibility into operational efficiency and production stability

### Data Model

A star schema was implemented to support efficient manufacturing analytics and KPI calculation.

- **Fact tables:** `fact_production`, `fact_maintenance`
- **Dimension tables:** `dim_customer`, `dim_product`, `dim_material`, `dim_machine`, and a custom `Date Table`

This structure enables analysis of production performance, quality metrics, and operational efficiency across multiple dimensions.

### Key DAX measures
Over 15 DAX measures were created to power the dashboard's visuals. Key measures include:

**Financial metrics:**
```dax
Total Revenue = SUM(Production[sales_price_per_board_usd] * Production[quantity_shipped])

Total Cost = SUM(Production[material_cost_usd] + Production[labor_cost_usd] + Production[maintenance_cost_usd])

Total Profit = [Total Revenue] - [Total Cost]

Profit Margin % = DIVIDE([Total Profit], [Total Revenue], 0)

YoY Revenue Growth % = 
VAR CurrentYearRevenue = [Total Revenue]
VAR PreviousYearRevenue = CALCULATE([Total Revenue], SAMEPERIODLASTYEAR('Date Table'[Date]))
RETURN DIVIDE(CurrentYearRevenue - PreviousYearRevenue, PreviousYearRevenue, 0)
```

**Quality metrics:**
```dax
Scrap Rate % = DIVIDE(SUM(Production[scrapped_units]), SUM(Production[units_produced]), 0)
```

**Operational metrics:**
```dax
Total Maintenance Cost = SUM(Maintenance[Labor Cost USD]) + SUM(Maintenance[Parts Cost USD])

Total Breakdowns = CALCULATE(COUNTROWS(Maintenance), Maintenance[Maintenance Type] IN {"Emergency", "Corrective"})

Breakdown Rate % = DIVIDE([Total Breakdowns], COUNTROWS(Maintenance), 0)
```

### Tools & Technologies
- **Power BI desktop:** For data modeling, DAX measure creation, and report visualization.
- **PostgreSQL:** The source relational database for the raw data.
- **DAX Studio:** Used for optimizing and debugging complex DAX measures.
- **AI (ChatGPT/LLM):** Used for generating the synthetic dataset.

---

##  How to use this repository

1.  **Clone the repository:** `git clone https://github.com/your-username/power-bi-hdi-manufacturing.git`
2.  **Open the power BI file:** The `.pbix` file contains the full report.
3.  **Explore the data model:** Review the relationships in the Model view.
4.  **Analyze the DAX measures:** The measures are organized in the `_Measures` table for clarity.

*Note: The data is imported into the Power BI file, so no external database connection is required to view the report.*

---

## What This Project Demonstrates

This project demonstrates the ability to:

- Design manufacturing data models for production analytics
- Build KPI-driven dashboards for quality and operations
- Apply DAX for manufacturing performance metrics
- Translate production data into actionable insights

## Future Enhancements

Potential improvements for this project:

1. **Customer Analysis Page** - Add a fourth page analyzing revenue by customer, customer retention, and geographic distribution
2. **Predictive Analytics** - Incorporate forecasting for maintenance costs and scrap rates
3. **Drill-through Pages** - Add detailed drill-through pages for specific machines or materials
4. **Mobile Layout** - Optimize the dashboard for mobile viewing
5. **Real-time Data** - Connect to a live database for real-time monitoring
6. **Bookmarks** - Add bookmarks for different analytical scenarios

---

##  License

This project is licensed under the MIT License - see the LICENSE file for details.

---

##  Connect With Me

I'm always interested in connecting with fellow data professionals and learning from the community!

- **LinkedIn:** www.linkedin.com/in/abdelkarim-mars-152570b5
- **GitHub:** https://github.com/KarimTheAnalyst 
- **Email:** karimupds@gmail.com

---

##  Acknowledgments

- **Power BI Community** - For countless tutorials and best practices
- **AI Tools** - For generating the synthetic dataset used in this project
- **Manufacturing Domain Experts** - For insights into PCB manufacturing processes and KPIs

---

