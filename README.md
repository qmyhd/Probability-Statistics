# Probability-Statistics
This repository contains various probability and statistics demonstrations, showcasing key concepts in statistical analysis, probability distributions, and theorems. The projects include simulations, visualizations, and statistical analysis using Python libraries like NumPy, SciPy, Matplotlib, and Seaborn.

## 🚀 Topics Covered:
- **Exploratory Data Analysis (EDA)**: Cleaning & visualizing datasets
- **Probability Distributions**: Binomial, Normal, and Poisson distributions
- **Statistical Inference**: Hypothesis testing, confidence intervals
- **Regression Models**: Linear Regression, Polynomial Regression, KNN Regression
- **Machine Learning Basics**: Clustering (K-Means), Decision Trees, and more


## 🔹 Code Samples:
### 🏎️ Example: Removing Outliers from Car Price Data
```python
import pandas as pd

def remove_outliers(df, column):
    Q1 = df[column].quantile(0.25)
    Q3 = df[column].quantile(0.75)
    IQR = Q3 - Q1
    lower_bound = Q1 - 1.5 * IQR
    upper_bound = Q3 + 1.5 * IQR
    return df[(df[column] >= lower_bound) & (df[column] <= upper_bound)]

cars_cleaned = remove_outliers(cars_data, 'Price')
```
###  Example: Visualizing Kernel Density of Car Prices
```python
import matplotlib.pyplot as plt
import seaborn as sns

plt.figure(figsize=(8, 6))
sns.kdeplot(cars_cleaned['Price'], fill=True)
plt.title('Kernel Density Plot of Car Prices')
plt.xlabel('Price')
plt.ylabel('Density')
plt.show()
```
