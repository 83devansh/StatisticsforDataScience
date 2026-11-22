# Practical 9: K-Nearest Neighbors (KNN) Classification Using Iris Dataset

## Objective
To implement the K-Nearest Neighbors (KNN) algorithm on the Iris dataset and evaluate its performance using accuracy, confusion matrix, and classification report.

## 1. Importing Libraries and Dataset

Imported the required libraries:
- Pandas
- Matplotlib
- Scikit-learn

Loaded the Iris.csv dataset and displayed the first five rows.

## 2. Data Exploration

Used the following functions:
- `head()` to display the first five rows.
- `columns` to display column names.
- `describe()` to get statistical information.
- `groupby()` to calculate the average measurements of each species.
- `size()` to count the number of samples in each species.

**Dataset Information:**
- Total observations: 150
- Total columns: 6
- Species: Iris-setosa, Iris-versicolor, Iris-virginica
- Each species contains 50 samples.

## 3. Feature Selection

- Independent variables (X): SepalLengthCm, SepalWidthCm, PetalLengthCm, PetalWidthCm and Id.
- Dependent variable (y): Species.

The Species column is used as the target variable for classification.

## 4. Splitting the Dataset

Divided the dataset into training and testing data using `train_test_split()`.

- Training data: 80%
- Testing data: 20%
- Random state: 42

## 5. Feature Scaling

Used StandardScaler to scale the training and testing data. Feature scaling helps KNN calculate distances more effectively because it is based on distance measurements.

## 6. Building the KNN Model

Created a KNN classifier using:

- Number of neighbors (K): 5

Trained the model using the training dataset and predicted the species of the test dataset.

## 7. Confusion Matrix

**Results:**

| Species | Correct Predictions |
|---|---:|
| Iris-setosa | 10 |
| Iris-versicolor | 9 |
| Iris-virginica | 11 |
| Total | 30 |

The confusion matrix shows that all 30 test samples were classified correctly.

## 8. Model Accuracy

**Result:**
- Accuracy: 100%

The model correctly classified all 30 test samples.

##