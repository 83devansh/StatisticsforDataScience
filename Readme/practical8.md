# Diabetes Prediction Using Decision Tree

## Overview
This project uses a Decision Tree Classifier to analyze the diabetes dataset and predict whether a person has diabetes based on various medical and health-related features. It also explores decision tree concepts such as entropy, information gain, and the Gini index.

## Dataset
The dataset contains 768 records and 9 columns, including 8 input features and 1 target variable.

### Features
- Pregnancies
- Glucose
- BloodPressure
- SkinThickness
- Insulin
- BMI
- DiabetesPedigreeFunction
- Age

### Target Variable
- `Outcome` — 0 indicates no diabetes, and 1 indicates diabetes.

## Objectives
- Explore and understand the dataset.
- Display statistical summaries.
- Separate independent and dependent variables.
- Split data into training and testing sets.
- Build a Decision Tree Classifier using entropy.
- Visualize the decision tree.
- Identify the root node and threshold.
- Calculate entropy and information gain.
- Calculate the Gini index.

## Technologies Used
- Python
- Pandas
- Matplotlib
- Scikit-learn

## Analysis Performed

### 1. Data Exploration
Loaded the diabetes dataset using Pandas and examined the first few rows, column names, and statistical summaries.

### 2. Feature Selection
Separated the independent variables (`X`) from the dependent variable (`y`), where `Outcome` is the target variable.

### 3. Train-Test Split
Split the dataset into:
- Training data: 80% (614 records)
- Testing data: 20% (154 records)

Used `random_state=42` for reproducibility.

### 4. Decision Tree Model
Built a Decision Tree Classifier using the entropy criterion and trained it on the training dataset.

### 5. Decision Tree Visualization
Visualized the trained decision tree using Matplotlib to understand the decision-making process and feature-based splits.

### 6. Root Node Analysis
Identified the root node selected by the trained model and its splitting threshold.

### 7. Entropy
Calculated the entropy of the root node to measure the uncertainty present in the target classes before the first split.

### 8. Information Gain
Calculated the information gain of the root split to measure how much uncertainty was reduced after splitting the data.

### 9. Gini Index
Trained another Decision Tree using the Gini criterion and calculated the impurity of the root node.

## Results

| Metric | Value |
|---|---:|
| Total records | 768 |
| Features | 8 |
| Training records | 614 |
| Testing records | 154 |
| Root node feature | Insulin |
| Root threshold | 121.0 |
| Root entropy | 0.9313 |
| Information gain | 0.3447 |
| Root Gini index | 0.4531 |

## Conclusion
This project demonstrates how a Decision Tree Classifier can be used for diabetes classification. It explores how the model selects features for splitting using entropy and information gain, and how Gini impurity measures the purity of a node.

The decision tree visualization helps understand how the model makes decisions based on different health-related features.

## How to Run
1. Open the notebook in Google Colab or Jupyter Notebook.
2. Place `diabetes.csv` in the working directory.
3. Install the required libraries:

   ```bash
   pip install pandas matplotlib scikit-learn
   ```

4. Run all cells in sequence.

