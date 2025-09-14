# UK-Energy-Consumption-Analysis
Business question: "Which regions of the UK show the highest and most inefficient energy consumption, and where should the company prioritise interventions to improve infrastructure capacity and sustainability?"

This project analyses regional energy consumption across the UK using an end-to-end workflow consisting of the tools Python, SQL and Power BI.
The goal is to uncover patterns in energy demand, identify areas of inefficiency and provide business and sustainability insights for stakeholders.

## Project Context

Energy consumption is a critical challenge for both businesses and sustainability efforts.
This project explores postcode-level and regional gas consumption data to answer questions such as:

- Which regions consume the most energy?
- Where is consumption disproportionately high relative to the number of meters?
- Are there areas with unusual distribution patterns (outliers)?
- How can this information guide infrastructure planning and sustainability initiatives?

## Data

Source: Government UK energy consumption data (cleaned and aggregated).
Size: ~1 billion postcode-level records.

Cleaning: Removed duplicate and aggregate rows (e.g., "All postcodes" entries), changed columns and handled nulls using Python.
Standardised region–postcode mapping and created ranking buckets (NTILE) for priority analysis using SQL.

## Tools & Techniques

- Python - Data cleaning and pre-processing.
- SQL – Data cleaning and data analysis.
- Power BI – Dashboard design, visualisation and KPI reporting.
- DAX Measures – Custom calculations

## Dashboard Preview


## Key Insights

- Total UK consumption in 2021 exceeded 589 billion kWh.
- Birmingham emerged as one of the highest-consuming regions, with over 20 billion kWh.
- Regions with a wide gap between mean and median consumption indicate unequal usage patterns — likely industrial hotspots.
- Certain areas show relatively few meters but very high per-meter consumption, suggesting heavy industrial use or inefficiencies.
- Colour-coded scatter plots clearly highlight regions consuming above the national average, making it easy for stakeholders to see which regions to target.

## Business & Sustainability Impact

- Business Planning: Helps energy providers allocate infrastructure and resources to high-demand regions.
- Sustainability: Identifies priority areas for energy efficiency programs and potential carbon reduction strategies.

## Next Steps

- Expand analysis with time-series data (monthly/quarterly).
- Compare with renewable energy adoption to measure sustainability impact.

## Files

Power Bi Dashboard - [Download Dashboard (.pbix)](./dashboard.pbix)  
Dataset- [View Cleaned Dataset](./example.csv)
