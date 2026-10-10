# U.S. Interest Rates and Housing Market Analytics

## Overview

I wanted to explore how interest rates and the U.S. housing market have changed over time. In this project, I used monthly data from January 2000 to August 2026 to look at federal funds rates, mortgage rates, housing starts, and new home sales.

I used Python to clean and explore the data, SQL to summarize trends and compare different interest rate environments, and Power BI to present the results visually.

## Questions I Explored

- How have federal funds rates and mortgage rates changed over time?
- How closely are the two rates related?
- How have housing starts and new home sales changed over the same period?
- How does housing activity compare between months with relatively high and low federal funds rates?

## Tools

- Python (Pandas)
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

Housing starts and new home sales are measured in thousands using seasonally adjusted annual rates (SAAR). The 2026 data only includes January through August.

## What I Found

- The average federal funds rate was 2.05%, and the average mortgage rate was 5.24%.
- The correlation between federal funds rates and mortgage rates was about 0.82 in the monthly data.
- Housing starts and new home sales had a correlation of about 0.93.
- The high-rate group had higher average housing starts and new home sales than the low-rate group in this dataset.

The last finding was not what I would automatically expect from the relationship between interest rates and housing demand. However, comparing averages alone does not explain why the difference exists. Other economic conditions and differences between time periods may also play a role.

## Project Files

- `01_data_cleaning.ipynb` — Data cleaning
- `02_data_merging.ipynb` — Combining the datasets
- `03_exploratory_analysis.ipynb` — Exploring trends and correlations
- `04_sql_analysis.ipynb` — SQL analysis using SQLite
- `sql/analysis.sql` — SQL queries used for the analysis
- `power_bi/` — Power BI dashboard PDF exports

## Limitations

This analysis looks at relationships in historical data, so the results do not establish cause and effect. Housing activity is also influenced by factors such as home prices, housing supply, affordability, and overall economic conditions. In addition, the 2026 data covers only eight months.

## Conclusion

This project gave me experience working through a data analysis workflow, from cleaning and combining data to using SQL for analysis and Power BI to communicate the results. It also showed me that relationships in economic data can be more complicated than they first appear.