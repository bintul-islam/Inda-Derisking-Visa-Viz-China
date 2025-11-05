# India's De-risking Paradox: Data-Driven Analysis and Visualization

## Project Overview

This project provides the implementation and data-driven analysis for the paper "India's De-risking Paradox: How Domestic Policy Deepens Strategic Dependence on China." It focuses on quantitatively examining India's trade relationships, specifically its imports and exports with China, to uncover patterns of dependency, assess the effectiveness of de-risking strategies, and visualize critical insights. The analysis identifies foundational trade imbalances, dissects the "illusion of diversification," and unveils the true extent of sector-specific dependencies as discussed in the paper.

## 1. Introduction: The Geoeconomic Challenge of an Adversarial Partner

India is pursuing a strategic de-risking initiative to address economic disparities and strategic vulnerabilities stemming from its complex relationship with China. This project provides the empirical examination of bilateral trade data, which is essential to move beyond rhetoric and accurately diagnose the scale and nature of India's economic vulnerability vis-à-vis China. The accompanying notebooks clean raw trade data, perform time-series analysis, and examine commodity-level import trends to support the paper's arguments regarding a "paradox of dependency" where domestic policies may inadvertently deepen reliance on China.

## 2. Project Structure

The project is organized into several directories and Jupyter notebooks to manage raw data, processed data, and analytical scripts effectively, mirroring the analytical sections of the paper.


## 3. Data Source

All raw trade data used in this analysis is publicly available from the World Integrated Trade Solution (WITS) platform, a product of The World Bank. Data for fiscal years (FY) 2003 through 2024 is utilized.

**Download Instructions:**
Data should be downloaded from [https://wits.worldbank.org/](https://wits.worldbank.org/) and placed into the `data/` directory as specified in the `Project Structure`.

*   **For Exports Data:**
    *   Select "Country-wise (Reports)", "Country (All)", and years "2003-2024".
    *   Save relevant files to `data/IndiaExportsChinaTotal`.
*   **For Imports Data:**
    *   Download all necessary data for "IndiaImportsAllCountries", "IndiaImportsChinaTotal", "IndiaImportsWorldTotal", and "ChapterImportWLD_CHN" for the specified years. These files are typically available by selecting different trade indicators and partner country aggregations on the WITS portal.

## 4. Notebooks: Quantifying the Asymmetry (Data-Driven Analysis)

This project includes several Jupyter notebooks, each designed to perform specific analyses that align with the quantitative sections of the paper.

### 4.1. `ImportExportAnalysis.ipynb` - Corresponds to Section 2.1: The Foundational Imbalance: An Exploding Trade Deficit

This notebook focuses on the high-level analysis of India's overall trade to establish the foundational trade imbalance, capturing the insights presented in Figure 1 of the paper.

*   **Time-series plots for imports and exports (Figure 1A):** Visualize the trends of India's total imports from and exports to China over time, demonstrating the dramatic divergence.
*   **Export-Import Ratio (Figure 1B):** Calculate and plot the ratio of exports to imports, illustrating the progressive decline in India's capacity to offset Chinese goods with its own productive output.
*   **Trade Deficit Severity (Figure 1C):** Plot the expanding trade deficit with China, underscoring the scale of the challenge.

### 4.2. `CountryDependence.ipynb` - Corresponds to Section 2.2: The Illusion of Diversification

This notebook delves into India's trade relationships with its top partners, particularly China, to deconstruct the "illusion of diversification" described in the paper and generate insights similar to Figure 2.

*   **Imports Country-level contribution charts (Figure 2A):** Generate visualizations showing the import share of India's top five partners, highlighting China's contribution.
*   **Dominance Index of China (Figure 2B):** Develop and visualize a dominance index quantifying China's import share relative to other top partners, assessing trends in its singular dominance.
*   **Combined Share of Top 5 Countries (Figure 2C):** Analyze the proportion of India's total world imports accounted for by the combined share of its top 5 partner countries.

### 4.3. `Commodity_Analysis.ipynb` - Corresponds to Section 2.3: Unveiling the True Dependency: A Sector-Specific Deep Dive

This notebook provides a detailed, granular look at commodity-level trade with China, unveiling the true extent of dependency in critical manufacturing value chains, as depicted in Figure 3.

*   **Top 5 Contributing Commodities (Imports from China) (Figure 3A):** Identify and visualize the top 5 commodities imported from China by volume and their respective share, focusing on core industrial goods (e.g., HS Code 85, 84, 29).
*   **% Growth Rate (CAGR) of these Commodities from China and World (Figure 3B):** Plot the Compound Annual Growth Rate (CAGR) for key product categories from China versus the world, indicating accelerating trade intensity.
*   **Diversity Vulnerability (Figure 3C):** Plot the number of products for which over 40% of India's total imports originate from China each year, illustrating the expanding breadth of supply chain vulnerability.

## 5. Results and Visualizations

The execution of these notebooks will generate a series of plots and data summaries that directly support the quantitative findings presented in the research paper. These visualizations serve as empirical evidence for the foundational imbalance, the illusion of diversification, and the deepening sector-specific dependencies.

## 6. Conclusion and Future Work

This project provides the computational framework for understanding India's de-risking paradox. The analysis reveals that superficial macro-level diversification often masks a deepening structural dependency on China, particularly in key manufacturing sectors. Future work could involve integrating policy data (e.g., PLI scheme details) to perform a more direct correlation analysis with the trade data trends, as hypothesized in Section 3 of the paper.
