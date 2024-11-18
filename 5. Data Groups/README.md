# Group 2: ✨ **Data Deamons** ✨ - Carbon Intensity Analysis for EcoFuture Analytics

This project analyzes the **carbon intensity (CI)** of commercial products from various sectors, using data provided by the **PCF-Database**. The goal of this analysis is to identify significant differences in CI across sectors, countries, and value chain stages to provide actionable insights for **Global Trade Alliance**. The analysis aims to inform sustainability strategies to reduce the environmental impact of global product distribution.

## Objective

The primary objectives of this analysis are:
- To identify **significant differences in carbon intensity** across sectors and countries.
- To analyze **value chain contributions** to carbon intensity, specifically upstream, operations, and downstream portions.
- To determine which portion of the value chain contributes most to **CI variability** across sectors.

## Data Sources

- **PCF-Database**: Contains data on carbon footprints (PCF) and carbon intensity (CI) of 866 commercial products from 8 industry sectors and 5 continents.
- **Carbon Intensity Data**: Sourced from [Figshare Collection](https://springernature.figshare.com/collections/The_Carbon_Catalogue_Carbon_footprints_of_866_commercial_products_from_8_industry_sectors_and_5_continents/5408100).

## Overall Key Findings of Analysis

### 1. Sectoral Differences in Carbon Intensity (CI)
- **Significant Differences**: Analysis revealed that CI varies significantly across sectors, confirmed through one-way ANOVA and post-hoc tests. Tukey’s test identified specific sector pairs with significant differences.
- **Overlapping Ranges**: Some sectors have overlapping CI ranges, making it challenging to distinguish their environmental performance through CI alone.
- **Reasons for Differences**:
  - Variability in industrial processes and energy efficiency.
  - Product lifecycle emissions differing by sector.

---

### 2. Regional and Country-Level Differences in CI
- **Significant Differences**: Differences in CI were observed among countries or regions. These differences highlight how local energy policies, industrial efficiency, and resource availability impact CI.
- **Potential Grouping**: Countries could be grouped based on renewable energy adoption, industrial maturity, or economic development for deeper insights.
- **Reasons for Variability**:
  - Geographic energy mix (e.g., renewable vs. non-renewable sources).
  - Technological adoption and efficiency standards.

---

### 3. Value Chain Contributions to CI
- **Analysis of Portions**: CI contributions from upstream, direct operations, and downstream portions were compared.
- **Significant Differences**: Statistical tests identified notable differences between these portions within sectors.
- **Reasoning**:
  - Upstream processes, like raw material extraction, generally exhibit higher variability due to dependence on natural resource conditions.
  - Operational differences arise from sector-specific efficiencies.

---

### 4. Largest Contributor to CI Variability Across Sectors
- The **upstream portion** was found to be the most significant driver of CI variability across sectors.
- **Reasons**:
  - Resource extraction methods differ substantially across sectors.
  - The energy mix used for upstream processes varies by sector.

---

## Visualizations
- Boxplots and bar plots were used to depict CI variance across sectors and value chain stages.
- These visualizations confirmed statistical findings and highlighted specific sectors and regions with extreme CI values.

---

## Final Recommendations

1. **Policy Focus on High CI Sectors**:
   - Target sectors with high average CI or overlapping CI ranges.
   - Prioritize sectors like manufacturing and transportation, which often have elevated CI.

2. **Mitigate Upstream Variability**:
   - Encourage the adoption of renewable energy sources and sustainable raw material extraction practices.
   - Implement stricter carbon footprint regulations for upstream activities.

3. **Regional Policies**:
   - Tailor strategies to regional differences in energy mix and industrial maturity.
   - Incentivize countries to adopt cleaner technologies and improve energy efficiency.

4. **Continuous Monitoring**:
   - Use statistical and visual tools regularly to evaluate progress in reducing CI.

By addressing these areas, the **Global Trade Alliance** can effectively reduce carbon intensity and enhance its global sustainability impact.

---

## Files in Repository

- **`group2_analysing_carbon_intensity_vF.ipynb`**  
  *This is the Jupyter Notebook containing the complete analysis of carbon intensity data for EcoFuture Analytics.*

- **`PublicTablesForCarbonCatalogueDataDescriptor_v30Oct2021.xlsx`**  
  *The primary dataset used for the analysis, containing product-level and stage-level carbon intensity data.*

- **`The Carbon Catalogue Article.pdf`**  
  *A detailed description of the dataset, methodology, and study context.*

---

## How to Use

1. Open the [Group2_analysing_carbon_intensity.ipynb](group2_analysing_carbon_intensity_vF.ipynb) notebook in JupyterLab or any compatible environment.
2. Ensure the required Python libraries (e.g., pandas, numpy, seaborn, matplotlib) are installed.
3. Run the notebook cells in order to reproduce the analysis and visualizations.
4. Review the findings in the provided visualizations and summary sections.

---

## Data Source

- The dataset used in this project was obtained from the [Carbon Catalogue](https://springernature.figshare.com/collections/The_Carbon_Catalogue_Carbon_footprints_of_866_commercial_products_from_8_industry_sectors_and_5_continents/5408100).
- A detailed description of the dataset and study can be found in [Carbon Catalogue Article.pdf](Carbon_catalogue_article.pdf).

---

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
```

---

## Contributors

- This analysis was conducted by the **Data Deamons** team (Group 2)

---