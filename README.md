# School-Age Connectivity Data Cleaning and Analysis

This project involves cleaning and analyzing a dataset related to internet connectivity among school-age children across various countries. The goal is to uncover patterns in digital access by region, wealth quintile, and residential area (urban vs rural) using Python.

## Project Overview

This analysis covers:

- Preprocessing and cleaning of structured tabular data
- Exploratory data analysis (EDA) using statistical methods
- Visualization of global disparities in home internet access
- Insight generation based on region, income level, and residence type

## Dataset Summary

The dataset contains information such as:

- Country and region identifiers
- Internet connectivity percentages (overall, urban, rural)
- Wealth quintile-based connectivity
- Income group and residence classifications
- Time period of data collection

## Data Cleaning Highlights

The following cleaning steps were performed:

- Removed leading and trailing spaces in string fields
- Identified and removed duplicate rows
- Standardized inconsistent labels in income group column
- Replaced out-of-range percentage values with null and later imputed
- Split time period into start and end year columns and removed invalid years
- Converted percentage fields from strings to integers
- Imputed missing values using region-wise means

The cleaned dataset is saved as:
```
cleaned_school_connectivity.csv
```

## Exploratory Data Analysis

### Internet Access by Region
- Europe and Central Asia shows the highest median access (~70%)
- Sub-Saharan Africa has the lowest median access (~10%)

### Access by Wealth Quintile
- Richest quintile has significantly higher access than the poorest
- Countries like Serbia and Chile show strong connectivity in both segments

### Urban vs Rural Analysis
- Urban median: 25.5%
- Rural median: 7.0%
- Mean internet access also higher in urban regions
- Both groups exhibit right-skewed distributions

## Visualizations

Plots were generated using:
- Boxplots for regional comparisons
- Bar charts for wealth group rankings
- Histograms and line plots for distribution comparisons

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

To install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn
```

## Files Included

- `school_connectivity_analysis.ipynb`: Main notebook with code
- `cleaned_school_connectivity.csv`: Final cleaned dataset
- `report_school_connectivity.pdf`: Summary report with findings
- `requirements.txt`: List of Python dependencies 