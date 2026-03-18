# Natural Gas Consumption Analysis

### Data Science & Predictive Modeling with Python

---

### Project Overview

**Natural Gas Consumption Analysis** is a data science project focused on identifying the meteorological and seasonal drivers of energy demand in North Carolina. The study analyzes the relationship between residential gas usage and key variables such as average temperature, **Heating Degree Days (HDD)**, and **Cooling Degree Days (CDD)**.

The project demonstrates a complete analytical pipeline: from data cleaning and exploratory visualization to statistical hypothesis testing and the implementation of high-accuracy machine learning regression models.

---

### Technologies Used

#### Data Analysis & Visualization
* **Python** – Core programming language.
* **Pandas & NumPy** – Data manipulation, cleaning, and matrix operations.
* **Matplotlib & Seaborn** – Advanced statistical data visualization (Heatmaps, Boxplots, Histograms).

#### Machine Learning & Statistics
* **Scikit-learn** – Implementation of Linear Regression models and performance metrics.
* **SciPy** – Statistical testing (Shapiro-Wilk normality test).
* **Regression Analysis** – Comparison between Simple and Multiple Linear Regression.

---

### Key Features

#### Exploratory Data Analysis (EDA)
* **Correlation Mapping:** Identified Heating Degree Days (HDD) as the primary driver of gas consumption ($R$ correlation near 1).
* **Seasonality Insights:** Categorical analysis of "Warm" vs. "Cold" months, revealing a drastic shift in median usage (from ~1,500 to ~12,000 units).
* **Distribution Profiling:** Detailed use of histograms and boxplots to visualize the right-skewed nature of residential energy demand.

#### Statistical Validation
* **Normality Testing:** Application of the Shapiro-Wilk test to confirm non-normal distribution ($p < 0.05$).
* **Feature Engineering:** Creation of specialized variables like `Warm_Month` and `Cooling_month` to capture non-linear seasonal effects.

#### Predictive Modeling
* **Model Comparison:** Evaluated a baseline Simple Regression against a Multiple Regression model.
* **High Precision:** Achieved an **$R^2$ score of 0.988** on training data and **0.981** on testing data.
* **Error Minimization:** Reduced Root Mean Squared Error (RMSE) by over 60% by transitioning to a multi-variable approach.

---

### Model Performance Results

| Metric | Simple Regression (Temp) | Multiple Regression (Temp+HDD+CDD) |
| :--- | :--- | :--- |
| **Train $R^2$** | 0.880 | **0.988** |
| **Test $R^2$** | 0.882 | **0.981** |
| **Test MAE** | 1342.86 | **561.12** |
| **Test RMSE** | 1676.11 | **665.38** |

---

### Project Conclusion

The analysis proves that residential gas consumption is almost entirely explained by weather variables. While temperature alone is a strong indicator, the inclusion of **Heating Degree Days** allows the model to capture the non-linear demand for heating during extreme cold. The resulting Multiple Regression model provides production-ready predictive accuracy, explaining over 98% of the variance in consumption.

---
