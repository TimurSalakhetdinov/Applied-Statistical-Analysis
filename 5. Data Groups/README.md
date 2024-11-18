# Carbon Intensity Analysis for EcoFuture Analytics

This project analyzes the **carbon intensity (CI)** of commercial products from various sectors, using data provided by the **PCF-Database**. The goal of this analysis is to identify significant differences in CI across sectors, countries, and value chain stages to provide actionable insights for **Global Trade Alliance**. The analysis aims to inform sustainability strategies to reduce the environmental impact of global product distribution.

## Objective

The primary objectives of this analysis are:
- To identify **significant differences in carbon intensity** across sectors and countries.
- To analyze **value chain contributions** to carbon intensity, specifically upstream, operations, and downstream portions.
- To determine which portion of the value chain contributes most to **CI variability** across sectors.

## Data Sources

- **PCF-Database**: Contains data on carbon footprints (PCF) and carbon intensity (CI) of 866 commercial products from 8 industry sectors and 5 continents.
- **Carbon Intensity Data**: Sourced from [Figshare Collection](https://springernature.figshare.com/collections/The_Carbon_Catalogue_Carbon_footprints_of_866_commercial_products_from_8_industry_sectors_and_5_continents/5408100).

## Analysis Tasks

### 1. Carbon Intensity Differences Among Sectors
- **Objective**: Are there significant differences in average carbon intensity (CI) among sectors?
- **Analysis**: ANOVA (F-test) was performed to identify sectors with significantly different CI.
- **Conclusion**: Significant differences in CI were observed, with some sectors showing higher CI values. Reasons for these differences include industry-specific production processes and geographical influences.

### 2. Carbon Intensity Differences Across Countries
- **Objective**: Are there significant differences in average CI across countries represented in the dataset?
- **Analysis**: A comparison of CI across different countries was made to highlight countries with significantly higher or lower CI values.
- **Conclusion**: Significant variation was found between countries, with developed nations showing lower CI due to more sustainable practices and technology adoption.

### 3. CI Contributions from Value Chain Portions
- **Objective**: Are there significant differences in CI contributions among the three value chain portions (upstream, operations, downstream)?
- **Analysis**: The variance in CI across the value chain portions was analyzed to identify where most of the carbon emissions come from within each sector.
- **Conclusion**: Upstream activities tend to contribute the most to CI in certain sectors, while downstream activities dominate others.

### 4. Value Chain Portion Driving CI Variability Across Sectors
- **Objective**: Which value chain portion contributes the most to CI variability across sectors?
- **Analysis**: ANOVA was used to test the variability of CI across the upstream, operations, and downstream portions for each sector.
- **Conclusion**: The **Upstream CO2e** portion contributed the most to CI variability across sectors, particularly in sectors like **Chemicals** and **IT**.

## Key Insights and Recommendations

- **Upstream CO2e** is the largest contributor to carbon intensity variability, suggesting that efforts to reduce emissions in the upstream stages of production could significantly reduce overall CI.
- Countries with lower CI should be encouraged to share best practices and technologies with nations that have higher CI to help reduce global emissions.
- Sectors like **Packaging for consumer goods** and **Construction materials** could focus on reducing CI in their downstream value chain portion for more efficient carbon reduction.

## Requirements

To run this Jupyter notebook and replicate the analysis, make sure you have the following Python libraries installed:

- `numpy`
- `pandas`
- `seaborn`
- `matplotlib`
- `scipy`
- `ipykernel`
- `stats`
- `pingouin`

You can install the necessary dependencies using `pip`:

```bash
pip install numpy pandas seaborn matplotlib scipy ipykernel stats pingouin