# House Price Prediction using Linear Regression

## Overview

This project demonstrates how to build a simple **Linear Regression** model using Python and Scikit-learn to predict house prices based on square footage.

Linear Regression is one of the most fundamental supervised machine learning algorithms used for predicting continuous numerical values. In this project, we train a model on a sample housing dataset, evaluate its performance, and visualize the regression results.

---

## Objectives

* Set up a Linear Regression model using Scikit-learn.
* Prepare and split data into training and testing sets.
* Train the model on historical data.
* Make predictions on unseen data.
* Evaluate model performance using MSE and R² Score.
* Visualize the regression line and actual data points.

---

## Technologies Used

* Python
* NumPy
* Pandas
* Scikit-learn
* Matplotlib

---

## Project Structure

```text
House-Price-Prediction/
│
├── linear_regression.py
├── README.md
└── requirements.txt
```

---

## Dataset

The sample dataset contains house prices based on square footage.

| Square Footage | Price ($) |
| -------------- | --------- |
| 1500           | 200000    |
| 1800           | 250000    |
| 2400           | 300000    |
| 3000           | 350000    |
| 3500           | 400000    |
| 4000           | 500000    |
| 4500           | 600000    |

---


## Model Workflow

### 1. Import Libraries

The project uses:

* NumPy for numerical operations
* Pandas for data manipulation
* Scikit-learn for machine learning
* Matplotlib for visualization

### 2. Load Dataset

The housing dataset is loaded into a Pandas DataFrame.

### 3. Split Data

The dataset is divided into:

* 80% Training Data
* 20% Testing Data

using `train_test_split()`.

### 4. Train Model

A Linear Regression model is initialized and trained:

```python
model = LinearRegression()
model.fit(X_train, y_train)
```

### 5. Make Predictions

Predictions are generated on the test dataset:

```python
y_pred = model.predict(X_test)
```

### 6. Evaluate Performance

The following metrics are used:

#### Mean Squared Error (MSE)

Measures the average squared difference between actual and predicted values.

```python
mean_squared_error(y_test, y_pred)
```

#### R-Squared (R²)

Measures how well the model explains the variance in the target variable.

```python
r2_score(y_test, y_pred)
```

---

## Visualization

The project generates a scatter plot of actual house prices along with the fitted regression line.

Features:

* Blue dots represent actual data points.
* Red line represents the predicted regression model.

---

## Sample Output

```text
Training data: (5,1), (5,)
Testing data: (2,1), (2,)

Intercept: 26785.71
Coefficient: 122.45

Predicted Prices:
[210459.18 594132.65]

Actual Prices:
[250000 600000]

Mean Squared Error: 781250000.0
R-squared: 0.95
```

*Note: Results may vary slightly due to train-test splitting.*

---

## Key Learning Outcomes

After completing this project, you will understand:

* Supervised Machine Learning fundamentals
* Linear Regression concepts
* Data preprocessing and train-test splitting
* Model training and prediction
* Performance evaluation using MSE and R²
* Data visualization techniques

---

## Future Enhancements

* Use larger real-world housing datasets.
* Add multiple input features (bedrooms, bathrooms, location, etc.).
* Implement Polynomial Regression.
* Compare Linear Regression with other ML algorithms.
* Deploy the model as a web application using Flask or FastAPI.

---

## Author

**Tejaswi**
Salesforce Developer | AI & Data Science Enthusiast | Data Engineer

---

## License

This project is open-source and available under the MIT License.
