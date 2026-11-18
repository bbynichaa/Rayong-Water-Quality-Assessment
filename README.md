# Rayong-Water-Quality-Assessment
Data-driven surface water quality assessment, pollution hotspot identification, and machine learning-based environmental management in Rayong Province (2018–2024).
# Surface Water Quality Assessment in Rayong Province (2018–2024)

## 1. Project Overview

This project integrates environmental engineering, data analytics, and machine learning to assess surface water quality and support pollution management in Rayong Province, Thailand.

## 2. Environmental Problem

Historical water quality monitoring data are available, but raw data alone make it difficult to identify pollution hotspots, understand pollution characteristics, and establish effective environmental management strategies.

## 3. Project Objectives

- Identify rivers and monitoring stations with poor water quality.
- Investigate spatial and temporal variations in water quality.
- Analyze relationships between pollution indicators.
- Estimate WQI using fewer water quality parameters.
- Simulate potential water quality improvement scenarios.

## 4. Dataset

- Study period: 2018–2024
- Total records: 447
- Monitoring stations: 27
- Study areas: Rayong River, Prasae River and Phang Rat River

Data source: https://rayong.gdcatalog.go.th/dataset/642d0ced-3f33-4c57-83a0-550050951ad6

### Water Quality Parameters

| Parameter | Description |
|---|---|
| DO | Dissolved Oxygen |
| BOD | Biochemical Oxygen Demand |
| TCB | Total Coliform Bacteria |
| FCB | Fecal Coliform Bacteria |
| NO3-N | Nitrate Nitrogen |
| NH3-N | Ammonia Nitrogen |
| WQI | Water Quality Index |

## 5. Data Cleaning and Transformation

- Data type validation
- Duplicate checking
- Buddhist Era to Gregorian calendar conversion
- Half reporting limit substitution
- Lower-bound substitution
- Training-based median imputation where required

## 6. Exploratory Data Analysis

- Descriptive statistics
- Boxplots
- Histograms
- Skewness analysis
- Scatterplots
- Pearson correlation
- Spearman correlation

The analysis revealed right-skewed pollutant distributions, extreme observations and relationships between water quality indicators.

## 7. Spatial and Temporal Analysis

The Rayong River exhibited the lowest historical average WQI among the three studied rivers.

Priority monitoring stations:

| Station | River | Historical Average WQI |
|---|---|---:|
| RY03 | Rayong River | 48.72 |
| PR04 | Phang Rat River | 47.11 |

Both stations exhibited persistent poor annual water quality throughout the seven-year study period.

## 8. Machine Learning

### Feature Selection

Input parameters were investigated using:

- Domain knowledge
- EDA-based feature selection
- Permutation feature importance

The selected reduced-parameter screening approach uses DO, BOD and NH3-N.

### Machine Learning Models

- Mean Baseline
- Linear Regression
- Polynomial Regression
- Decision Tree Regression
- Random Forest Regression

### Model Evaluation

- R-squared (R²)
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- Grouped cross-validation
- Temporal validation

Random Forest Regression was the best-performing algorithm in the latest corrected comparison using the selected three parameters. Final metrics should be confirmed from the submitted notebook.

## 9. Environmental Management and Improvement

A proposed WQI target of 65 was established for RY03 and PR04.

What-if scenario analysis was conducted to investigate potential improvements through:

- Increasing dissolved oxygen
- Reducing organic pollution
- Reducing ammonia concentrations

The simulation supports preliminary environmental management planning rather than establishing causal effects.

## 10. Real-world Applications

- Pollution hotspot identification
- Targeted environmental monitoring
- Preliminary water quality screening
- Resource-efficient monitoring strategies
- Station-specific pollution management
- Environmental decision support

## 11. Limitations

- Correlation does not imply causation.
- Monitoring coverage varies across years.
- Substituted measurements are approximations.
- Machine learning predictions require further independent validation.
- Simulated improvements do not guarantee actual environmental improvements.
- Reduced-parameter screening cannot replace regulatory water quality testing.

## 12. Tools and Technologies

- Microsoft Excel
- Google Colab
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- GitHub

## 13. Conclusion

This project demonstrates how environmental data analytics and machine learning can support targeted pollution management and more efficient water quality monitoring in Rayong Province.
