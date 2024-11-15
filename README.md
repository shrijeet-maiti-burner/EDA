# Digital Assignment for BCSE331L
## Expploratory Data Analysis and Model Evaluation

**Name:** Shrijeet Maiti  
**Roll No.:** 21BDS0144  

---

Involves extensive data analysis and visualization techniques applied to the [Catholic Dataset](https://raw.githubusercontent.com/salemprakash/EDA/main/Data/catholic.csv). Key data manipulation steps include merging, reshaping, transformation, binning, outlier detection, univariate and bivariate analysis, clustering, principal component analysis, and linear regression.

**GitHub Repository:** [Link to GitHub](https://github.com/shrijeet-maiti-burner/EDA/blob/master/21BDS0144.ipynb)

### Modules and Analysis Techniques

#### Module 1: Loading and Exploring the Dataset
- **Dimensions**: Understanding the structure with `.shape`
- **Summary Statistics**: Generated using `.describe()`
- **Data Types**: Checked with `.dtypes`

#### Module 2: Data Transformation and Cleaning
- **Merging Data**: Merged using the `id` column with an inner join.
- **Hierarchical Indexing**: Set hierarchical index with `id` and `female`.
- **Deduplication & Missing Values**:
  - Removed duplicates and handled missing values through various imputation techniques (mean, median, mode, forward/backward fill).
- **Discretization**: Equal-width and quantile-based binning on numerical columns.

#### Module 3: Univariate and Bivariate Analysis
- **Measures of Central Tendency**: Calculated mean, median, and mode.
- **Dispersion**: Calculated standard deviation, variance, and IQR.
- **Correlation Analysis**: Explored relationships between `read12` and `math12`.
- **Visualization**: Histograms, box plots, density plots, and pie charts.

#### Module 4: Multivariate Analysis
- **Categorical Plots**: Stacked bar plots and count plots for categorical comparisons.
- **Quantitative Relationships**: Scatter plots, correlogram, and bubble plots.
- **Advanced Visualization**: 3D scatter and bar plots, sunray plots.

#### Module 5: Clustering Analysis
- **K-Means Clustering**: Used the elbow method to determine optimal clusters.
- **Hierarchical Clustering**: Dendrograms with various linkage methods for clustering insight.

#### Module 6: Dimensionality Reduction
- **Principal Component Analysis (PCA)**: Performed PCA and visualized with scree plot and biplot.
- **Multidimensional Scaling (MDS)**: Mapped data to 2D space for distance preservation.

#### Module 7: Regression Analysis
- **Linear Regression**: Modeled `math12` scores based on `read12`, `motheduc`, `fatheduc`, and `lfaminc`.
- **Metrics and Interpretation**:
  - **R-squared** (R²): Indicating moderate predictive power.
  - **Mean Absolute Error (MAE)**: Showing the average prediction error.
  - **Mean Squared Error (MSE)**: Providing an error measure sensitive to larger discrepancies.
- **Multiple Linear Regression**: Log transformations on `math12` scores based on `read12`, `motheduc`, `fatheduc`, and `lfaminc`.
- **Prediction and Residual Analysis**:
  - Plots to compare predicted values and residuals.
  - **Shapiro-Wilk test**: Showing residual deviation from actual values.
  - **Q-Q Plot**: Confirming model's validity.