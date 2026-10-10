# U.S. Interest Rates and Housing Market Analytics

## Overview

I wanted to see how interest rates and the U.S. housing market have changed over time. For this project, I worked with monthly data from January 2000 to August 2026, focusing on federal funds rates, mortgage rates, housing starts, and new home sales.

I used Python to clean and explore the data, SQL to compare trends and interest rate periods, and Power BI to build dashboards.

## Questions I Explored

- How have federal funds rates and mortgage rates changed over time?
- How are the two rates related?
- How have housing starts and new home sales changed over the years?
- How does housing activity differ between periods with higher and lower federal funds rates?

## Tools

- Python (Pandas, Matplotlib)
- SQL (SQLite)
- Power BI
- Jupyter Notebook

## Data

The dataset includes 320 monthly observations from January 2000 through August 2026. It contains federal funds rates, 30-year mortgage rates, housing starts, and new home sales.

Housing starts and new home sales are measured in thousands using seasonally adjusted annual rates (SAAR). The 2026 data only covers January through August.

## What I Found

The average federal funds rate was 2.05%, compared with 5.24% for mortgage rates. The two rates had a correlation of about 0.82.

Housing starts and new home sales were also strongly correlated, with a correlation of about 0.93.

One result that stood out was that the high-rate group had higher average housing starts and new home sales than the low-rate group. This was not what I initially expected. However, interest rates are only one part of the housing market, and the difference in averages does not tell us what caused this result.

## Project Files

- `notebooks/01_data_cleaning.ipynb` — Cleaning the original datasets
- `notebooks/02_data_merging.ipynb` — Combining the datasets
- `notebooks/03_exploratory_analysis.ipynb` — Exploring trends and correlations
- `sql/04_sql_analysis.ipynb` — Analyzing the data with SQL
- `Power_Bi/Market_Overview_PowerBi.pdf` — Overall market trends
- `Power_Bi/Interest_Rate_Trends_PowerBi.pdf` — Interest rate trends
- `Power_Bi/Housing_Market_Analysis_PowerBi.pdf` — Housing market analysis

## Limitations

This project looks at historical relationships and does not prove that changes in interest rates caused changes in housing activity. Other factors, including home prices, housing supply, affordability, and broader economic conditions, can also affect the market. The 2026 data is incomplete because it only covers the first eight months.

## Conclusion

Through this project, I got experience with the full data analysis process, from cleaning and combining datasets to using SQL and building Power BI dashboards. I also learned that economic data can produce results that are not always as straightforward as expected.
