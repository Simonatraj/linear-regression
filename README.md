Linear Regression
Overview
This project implements a simple Linear Regression model from scratch using Python and NumPy. The model uses gradient descent to optimize the weights and bias for predicting continuous target values based on input features.
Features

Custom implementation of linear regression without relying on external machine learning libraries.
Configurable learning rate and number of iterations for gradient descent.
Supports multi-feature datasets for training and prediction.
Lightweight and easy to understand for educational purposes.

Requirements

Python 3.6 or higher
NumPy (pip install numpy)

Installation
Follow these steps to set up the project locally:

Clone the repository:git clone https://github.com/Simonatraj/linear-regression.git


Navigate to the project directory:cd linear-regression


Install dependencies:pip install numpy



Usage
The LinearRegression class can be used to train a model on a dataset and make predictions. Below is an example of how to use the code:
import numpy as np
from linear_regression import LinearRegression

# Sample data
X = np.array([[1, 2], [3, 4], [5, 6]])  # Feature matrix
y = np.array([3, 7, 11])               # Target values

# Initialize and train the model
model = LinearRegression(lr=0.01, n_iters=1000)
model.fit(X, y)

# Make predictions
X_test = np.array([[2, 3], [4, 5]])
predictions = model.predict(X_test)
print(predictions)

Parameters

lr: Learning rate for gradient descent (default: 0.0001)
n_iters: Number of iterations for gradient descent (default: 1000)

Example Output
For the above example, the output might look like:
[4.85, 8.92]

Notes

Ensure your input features (X) are a 2D NumPy array and the target values (y) are a 1D NumPy array.
The model assumes a linear relationship between features and target values.
You may need to tune the learning rate (lr) and number of iterations (n_iters) for optimal convergence, depending on your dataset.

