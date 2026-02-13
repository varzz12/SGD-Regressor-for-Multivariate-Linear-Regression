# SGD-Regressor-for-Multivariate-Linear-Regression

## AIM:
To write a program to predict the price of the house and number of occupants in the house with SGD regressor.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Data Preprocessing & ScalingLoad your dataset and separate your features (X) from your targets (y1 for Price, y2 for Occupants). You must apply feature scaling (like StandardScaler) to your input features; otherwise, the gradient descent might fail to converge or take far too long.
2. 2. Model InitializationSince a standard SGD Regressor typically handles one output at a time, you have two options:Multi-Output Wrapper: Wrap the SGDRegressor in a MultiOutputRegressor to handle both targets simultaneously.Independent Models: Initialize two separate instances of SGDRegressor, one tuned for price and one for occupancy.
3. Iterative Training (Fit)Train the model using the .fit() method. The SGD algorithm will iteratively update the weights by calculating the gradient of the loss function for each sample (or small batches), moving toward the global minimum of the cost function.
4. Prediction & EvaluationPass new house features into the .predict() method. Evaluate the performance using Mean Squared Error (MSE) or R-squared for both the Price and Occupant predictions to ensure the model isn't biased toward one specific target.

## Program:
```
/*
Program to implement the multivariate linear regression model for predicting the price of the house and number of occupants in the house with SGD regressor.
Developed by: 
RegisterNumber:  
*/
```

## Output:
![multivariate linear regression model for predicting the price of the house and number of occupants in the house](sam.png)


## Result:
Thus the program to implement the multivariate linear regression model for predicting the price of the house and number of occupants in the house with SGD regressor is written and verified using python programming.
