# Life Expectancy and Model Reduction Analysis

## Project Overview
This project explores a dataset related to life expectancy and its associated factors, focusing on model reduction techniques. The primary goal is to reduce a model using both p-values and AIC, evaluate the results, and compare them across different train-test splits.

---

## Dataset
- **Name**: Life Expectancy Data
- **Source**: World Health Organization (WHO). The dataset was obtained from [Kaggle](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who).
- **Description**: This dataset includes factors such as income composition, schooling, immunization, and more, which are analyzed to understand their effect on life expectancy.

---

## Key Steps in Analysis

### 1. Data Preprocessing
- Load the dataset and clean column names for better readability.
- Remove redundant features and address multicollinearity among variables.
- Impute missing values where necessary to ensure a complete dataset for analysis.

### 2. Model Reduction
- **Methods Used**:
  1. Reduction based on **p-values**:
     - Sequentially remove features with the highest p-value greater than a specified threshold (e.g., 0.05).
  2. Reduction based on **AIC**:
     - Iteratively remove features to minimize the Akaike Information Criterion (AIC).
- **Evaluation**:
  - Models were compared using metrics such as Mean Squared Error (MSE), R², and AIC.

### 3. Splitting and Validation
- The most parsimonious model (from AIC reduction) was used for further validation.
- Train-test splits with varying proportions (10:90, 30:70, 50:50) were tested to evaluate the model's performance consistency.

---

## Key Results

### Model Reduction Metrics
| Model Type       | MSE    | R²     | AIC       |
|-------------------|--------|--------|-----------|
| p-values Model    | 18.870 | 0.7822 | 13961.716 |
| AIC Model         | 18.659 | 0.7846 | 13960.460 |

### Splitting Results (AIC Model)
| Train:Test Split  | MSE    |
|--------------------|--------|
| 10:90              | 19.366 |
| 30:70              | 19.491 |
| 50:50              | 19.447 |

---

## Key Takeaways
- The AIC-based model reduction approach proved to be more effective in balancing model complexity and performance.
- The GLM with a Gamma family and log link is well-suited for predicting life expectancy, given its non-normal distribution.

---

## Libraries Used
- `pandas`
- `numpy`
- `statsmodels`
- `sklearn`
- `matplotlib`
- `seaborn`

---

## File Structure
- Model_reduction.ipynb: The main notebook with all analyses and results.
- Life Expectancy Data.csv: Dataset used for the analysis.

---

## How to Use
1.	Clone the repository and navigate to the project folder.
2.	Ensure all required libraries are installed:

```bash
pip install pandas numpy statsmodels scikit-learn matplotlib seaborn
```

3.	Run the Jupyter Notebook:

```bash
jupyter notebook Model_reduction.ipynb
```

---

## Contributors

- This analysis was conducted by the **Data Demons** team (Group 2)

---