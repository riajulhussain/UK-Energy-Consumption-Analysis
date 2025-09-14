# UK Energy Consumption Analysis
**Business question: "Which areas of the UK present the best opportunities for targeted investment in metering infrastructure to relieve pressure on energy demand and improve long-term sustainability?"**

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

Source: Government UK energy consumption data.
Size: ~1 billion postcode-level records.

Cleaning: Removed duplicate and aggregate rows (e.g., "All postcodes" entries), changed columns and handled nulls using Python.
Standardised region–postcode mapping and created ranking buckets using CTEs and Window Functions for priority analysis using SQL.

## Tools & Techniques

- Python - Data cleaning and pre-processing.
- SQL – Data cleaning and data analysis.
- Power BI – Dashboard design, visualisation and KPI reporting.
- DAX Measures – Custom calculations

## Dashboard Preview

![Dashboard Preview](https://github.com/riajulhussain/UK-Energy-Consumption-Analysis/blob/main/Screenshot%202025-09-14%20172356.png)


 ## Dashboard Walkthrough (for non-technical stakeholders)

This dashboard was designed to answer the business question:  
**"Which areas of the UK present the best opportunities for targeted investment in metering infrastructure to relieve pressure on energy demand and improve long-term sustainability?"**

### 1. KPI Cards
- Total UK Consumption: Shows overall demand across the UK.
- Average Consumption per Meter: Averages usage across households/meters, useful to spot efficiency levels.  
- Birmingham Total Consumption: Highlights a high-consumption city to show regional concentration.  

### 2. Bar Chart – Top 10 Regions by Total Consumption
- Quickly shows which regions consume the most energy.  
- Helps identify priority regions for infrastructure investment.  

### 3. Scatter Plot – Avg. Consumption per Meter vs. Total Meters
- Each point is a region, colour-coded red/green depending on whether they are above/below the national average.  
- Shows where consumption is unusually high given the number of meters - possible inefficiencies or industrial hotspots.  

### 4. Histogram – Distribution of Average Consumption
- Shows how average consumption is spread across regions.  
- Helps identify outliers.

### 5. Top Suggested Regions – Based on Meter Availability and Consumption Rankings

This chart shows the top 17 regions most in need of infrastructure improvements, based on three key factors:
- Total energy consumption – how much energy is used overall.
- Number of installed meters – how many customers/meters are in the region.
- Average consumption per meter – how much energy the area consumes typically.

To make this easy to compare, each region is given a score (rank). A higher rank means the region has relatively high consumption but fewer meters, suggesting the infrastructure might be under pressure.

Why it matters for the business:
This chart highlights where the company should take priority. If a region uses a lot of energy but has fewer meters, it could mean:
- Strain on existing infrastructure
- High-value customers concentrated in one area
- Opportunity to expand metering coverage to balance demand

So, instead of treating all regions equally, the chart prioritises areas where action will have the biggest impact.
 
## Key Insights

- Total UK consumption in 2021 exceeded 589 billion kWh.
- Birmingham emerged as one of the highest-consuming regions, with over 20 billion kWh.
- Certain areas show relatively few meters but very high per-meter consumption, suggesting heavy industrial use or inefficiencies.
- Colour-coded scatter plots clearly highlight regions consuming above the national average, making it easy for stakeholders to see which regions to target.
- Birmingham, Guildford, Leicester and Blackburn are among the list that stand out as areas with high energy consumption but relatively fewer meters installed, indicating that these areas would be key in installing more meters.

## Business & Sustainability Impact

- Business Planning: Helps energy providers allocate infrastructure and resources to high-demand regions.
- Sustainability: Identifies priority areas for energy efficiency programs and potential carbon reduction strategies.

## Next Steps

- Expand analysis to monitor energy demand by year.
- Compare with renewable energy to measure sustainability impact.

## Files

Power BI Dashboard - [Download Dashboard (.pbix)]([./dashboard.pbix](https://github.com/riajulhussain/UK-Energy-Consumption-Analysis/blob/main/Energy%20Consumption%20Dashboard.pbix))  
Dataset- [View Cleaned Dataset]([./example.csv](https://github.com/riajulhussain/UK-Energy-Consumption-Analysis/blob/main/original_table.energy.csv))

Feel free to connect! - [LinkedIn](http://www.linkedin.com/in/riajulhussain)
