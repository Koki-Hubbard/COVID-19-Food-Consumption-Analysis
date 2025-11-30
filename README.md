# Food Retail Dashboard: COVID-19 Impact & Recovery Timeline

## Overview
Food retailers faced unexpected volatility during the COVID-19 pandemic, lacking clear insight in category specific patterns. This dashboard analyzes year-over-year spending across 20 food categories in order to quantify the March 2020 shock and recovery timeline through December 2020. This analysis reveals that while all categories saw a dramatic 20-27% spike initially, the recovery timeline varied from category to category with some categories like fresh produce (fruits & vegetables) taking up to 6+ months to normalize while others stablized within 30 days. 

## Business Problem
Stakeholder: Supply Chain & Category Management Teams at grocery retailers
March 2020 created a supply & demand mismatch across all food categories leaving retailers unsure about which categories required a short term or a long term inventory buffer without the correct strategies in place. Which categorie recovered the fastest? Should we maintain higher safety stock levels for all food categories or prioritize specific areas?

## Methodology 
### Data Transformation
- Calculated year-over-year % change using 12-month lookback function to account for seasonal changes
- Filtered to 2020 data while retaining 2019 baseline for comparison logic
- Aggregated 20 sub-categories from BEA's Personal Consumption Expenditures dataset

### Analysis 
- Identified top 5 disrupted categories by ranking March 2020 YoY% values
- Built recovery timeline tracking these categories across Mar/May/Aug/Dec checkpoints
- Used WINDOW_AVG() calculations to retrieve summary KPIs (average shock, recovery rate)

## Key Findings  & Recommendations
### Insights
- Fresh produce showed sustained elevation:  Fresh fruit and vegetables remained 13-18% above 2019 baseline through December, indicating long-term behavioral shifts toward home cooking
- Recovery correlated with product type: Essential food items (proteins, produce) took 4-6 months to stabilize while discretionary items (alcohol, sweets) normalized within 30-45 days
- Fast initial rebound: By May 2020, categories had recovered 45-60% of their March spike, suggesting demand stabilization occurs faster than supply chain adjustment
- Large variance by category: Peak disruption ranged from 21% (sugar/sweets) to 27% (fresh fruit), meaning a generic inventory strategy would have been costly

### Recommendations
- Safety stock by category type: Maintain 15-20% buffer for fresh produce; reduce to 5-10% for discretionary items during disruption events
- Implement monitoring windows: Most categories stabilize within 2 months post-shock with some exceptions (fresh produce) require extended 4-6 month plans

## Skills Demonstrated
- **Tableau** - Dashboard design, calculated fields, table calculations
- **Excel** - Initial data validation and structure review

## Tools Used
-Tableau Desktop 
-Excel 
-Bureau of Economic Analysis (BEA) Data — Personal Consumption Expenditures (2016-2021)

---

## Project Files


