# U.S. Interest Rates and Housing Market Analytics

## Overview

I wanted to explore how interest rates and the U.S. housing market have changed over time. In this project, I used monthly data from January 2000 to August 2026 to examine federal funds rates, mortgage rates, housing starts, and new home sales.

I used Python to clean and explore the data, SQL to summarize trends and compare different interest rate environments, and Power BI to present the results visually.

## Questions I Explored

- How have federal funds rates and mortgage rates changed over time?
- How closely are the two rates related?
- How have housing starts and new home sales changed over the same period?
- How does housing activity compare between months with relatively high and low federal funds rates?

## Tools

- Python (Pandas, Matplotlib)
- SQL (SQLite)
- Power BI
- Jupyter Notebook

## Data

The dataset contains 320 monthly observations from January 2000 through August 2026.

| Column | Description |
|---|---|
| `date` | Monthly date |
| `fed_funds_rate` | Federal funds rate (%) |
| `mortgage_rate` | 30-year mortgage rate (%) |
| `housing_starts` | Housing starts (thousands, SAAR) |
| `new_home_sales` | New home sales (thousands, SAAR) |

Housing starts and new home sales are measured in thousands using seasonally adjusted annual rates (SAAR). The 2026 data covers January through August only.

## What I Found

- The average federal funds rate was 2.05%, while the average mortgage rate was 5.24%.
- The correlation between federal funds rates and mortgage rates was approximately 0.82.
- Housing starts and new home sales had a correlation of approximately 0.93.
- In this dataset, the high-rate group had higher average housing starts and new home sales than the low-rate group.

The last finding was not what I would automatically expect from the relationship between interest rates and housing demand. However, comparing averages alone does not explain why the difference exists. Other economic conditions and differences between time periods may also play a role.

## Project Files

- `notebooks/01_data_cleaning.ipynb` — Data cleaning
- `notebooks/02_data_merging.ipynb` — Combining the datasets
- `notebooks/03_exploratory_analysis.ipynb` — Exploring trends and correlations
- `sql/04_sql_analysis.ipynb` — SQL analysis using SQLite
- `Power_Bi/Market_Overview_PowerBi.pdf` — Market overview dashboard
- `Power_Bi/Interest_Rate_Trends_PowerBi.pdf` — Interest rate trends dashboard
- `Power_Bi/Housing_Market_Analysis_PowerBi.pdf` — Housing market analysis dashboard

## Limitations

This analysis examines relationships in historical data and does not establish cause and effect. Housing activity is also influenced by factors such as home prices, housing supply, affordability, and overall economic conditions. In addition, the 2026 data covers only eight months.

## Conclusion

This project gave me experience working through a data analysis workflow, from cleaning and combining data to using SQL for analysis and Power BI to communicate the results. It also showed me that relationships in economic data can be more complicated than they first appear.

## About

An analysis of U.S. interest rates and housing market trends using Python, SQL, and Power BI.
