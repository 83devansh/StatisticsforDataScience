# Wine Dataset Analysis and PCA

## Overview
This project performs Exploratory Data Analysis (EDA) and Principal Component Analysis (PCA) on the Wine dataset using Python. It analyzes different chemical properties of wine, visualizes the data, scales the features, and reduces dimensionality using PCA.

## Dataset
The dataset contains 178 wine samples with 13 numerical features and one target column (`Class`).

Features include:
- Alcohol
- Malic Acid
- Ash
- Alcalinity of Ash
- Magnesium
- Total Phenols
- Flavanoids
- Nonflavanoid Phenols
- Proanthocyanins
- Color Intensity
- Hue
- OD280/OD315 of Diluted Wines
- Proline

## Objectives
- Display statistical summaries of the dataset.
- Analyze alcohol content across wine classes.
- Visualize the relationship between alcohol and color intensity.
- Calculate and visualize the covariance matrix.
- Standardize the dataset using StandardScaler.
- Reduce dimensionality using PCA.
- Visualize wine class separation using two principal components.

## Technologies Used
- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Analysis Performed
1. **Statistical Analysis:** Used `df.describe()` to view mean, standard deviation, minimum, maximum, and quartile values.
2. **Boxplot:** Compared alcohol content across different wine classes.
3. **Scatterplot:** Visualized the relationship between alcohol and color intensity.
4. **Covariance Matrix:** Analyzed relationships between numerical features.
5. **Feature Scaling:** Applied StandardScaler to standardize the data.
6. **PCA:** Reduced 13 features into 2 principal components for visualization.

## Results
- The dataset contains 178 samples and 13 numerical features.
- PCA reduced the original 13 features to 2 components.
- The first principal component explains approximately 36.20% of the variance.
- The second principal component explains approximately 19.21% of the variance.
- Together, both components explain **55.41% of the total variance**.

## How