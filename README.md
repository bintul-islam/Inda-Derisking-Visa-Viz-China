# Inda-Derisking-Visa-Viz-China

## Table of Contents
1.  Introduction
2.  Project Structure
3.  Data Source
4.  Notebooks
    *   `Import_Export_Data_Cleaning.ipynb`
    *   `Import_Export_Analysis.ipynb`
    *   `Chinese_Dependence.ipynb`
    *   `Commodity_Analysis.ipynb`
5.  Results and Visualizations (Example)
6.  Conclusion and Future Work

## 1. Introduction

This project aims to analyze India's trade data, with a specific focus on understanding and visualizing its trade relationships, particularly concerning imports and exports with China. The goal is to identify patterns, dependencies, and potential areas for "derisking" India's trade reliance on specific countries or commodities. This analysis will involve cleaning raw trade data, performing time-series analysis, and examining commodity-level import trends.

## 2. Project Structure

The project is organized into several directories to manage raw data, processed data, and notebooks effectively.

```
.
├── data/
│   ├── IndiaExportsChinaTotal
│   ├── IndiaImportsAllCountries
│   ├── IndiaImportsChinaTotal
│   ├── IndiaImportsWorldTotal
│   ├── ChapterImportWLD_CHN
├── ImportExportAnalysis.ipynb
├── CountryDependence.ipynb
├── ChapterWiseAnalysis.ipynb
├── README.md
```


## 3. Data Source

The raw data is expected to be in `.csv` format, downloaded ***https://wits.worldbank.org/***

### 3.1. For Exports Data
1.  Download the Exports data Select Country-wise(Reports) and Country(All) for years 2003-2024 and put in the **Directory: `data/`**

### 3.2. For Imports Data
1.  Download all relevant data from the website already downbload in the **data** folder

## 4. Notebooks

This project includes several Jupyter notebooks, each designed for a specific part of the data processing and analysis pipeline.


### 4.1. `ImportExportAnalysis.ipynb`
This notebook focuses on high-level analysis of India's overall trade:
1.  **Time-series plots for imports and exports**: Visualize the trends of India's total imports and exports over time.
2.  **Export-Import Ratio**: Calculate and plot the ratio of exports to imports to understand India's trade balance.
3.  **Trade Deficit Sevirity**: Plot 

### 4.3. `CountryDependence.ipynb`
This notebook dives deeper into India's trade relationship with China:
1.  **Imports Country-level contribution charts**: Generate visualizations showing the contribution of various countries to India's total imports, highlighting China's share.
2.  **Dominance Index of China**: Develop and visualize a dominance index to quantify India's reliance on China for imports.
3.  **Import share of top 5 countries**: Compare China's import share against other top importing countries.

### 4.4. `Commodity_Analysis.ipynb`
This notebook provides a detailed look at commodity-level trade with China:
1.  **Top 5 Contributing commodities (Imports) (CHINA)**: Identify and visualize the top 5 commodities imported from China.
2.  **% Growth rate of these commodies from china and world**: CAGR plot for key products world and china
3.  **Diversity Valnaurability**: Plot No of product whose 40% of imports are from china every year



