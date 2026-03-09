# SGD-Regressor-for-Multivariate-Linear-Regression

## AIM:
To write a program to predict the price of the house and number of occupants in the house with SGD regressor.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Initialize weights, bias, learning rate, and number of iterations.
2.Compute the predicted output using the sigmoid function.
3.Calculate gradients of the loss and update weights and bias using gradient descent.
4.Repeat the process until convergence or maximum iterations are reached.

## Program:
```
/*
import numpy as np
from sklearn.linear_model import SGDRegressor
from sklearn.multioutput import MultiOutputRegressor
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler
from sklearn.metrics import mean_squared_error

X = np.array([
    [800, 2],
    [1000, 3],
    [1200, 3],
    [1500, 4],
    [1800, 4],
    [2000, 5],
    [2200, 5],
    [2500, 6]
])
y = np.array([
    [40, 2],
    [55, 3],
    [65, 3],
    [85, 4],
    [95, 4],
    [110, 5],
    [125, 5],
    [145, 6]
])

X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.25, random_state=42
)

scaler = StandardScaler()
X_train_scaled = scaler.fit_transform(X_train)
X_test_scaled = scaler.transform(X_test)

sgd = SGDRegressor(
    max_iter=2000,
    eta0=0.01,
    learning_rate='constant',
    random_state=42
)

model = MultiOutputRegressor(sgd)

model.fit(X_train_scaled, y_train)

y_pred = model.predict(X_test_scaled)

print("Predicted [Price, Occupants]:")
print(y_pred)

print("\nActual [Price, Occupants]:")
print(y_test)


mse = mean_squared_error(y_test, y_pred)
print("\nMean Squared Error:", mse)

new_house = np.array([[1600, 4]])
new_house_scaled = scaler.transform(new_house)

new_prediction = model.predict(new_house_scaled)

print("\nFor New House [1600 sq ft, 4 rooms]:")
print("Predicted House Price (lakhs):", round(new_prediction[0][0], 2))
print("Predicted Number of Occupants:", round(new_prediction[0][1]))
import matplotlib.pyplot as plt

plt.figure()
plt.scatter(X_test[:, 0], y_test[:, 0], label="Actual Price")
plt.scatter(X_test[:, 0], y_pred[:, 0], label="Predicted Price")
plt.xlabel("House Size (sq ft)")
plt.ylabel("House Price (lakhs)")
plt.title("House Size vs House Price (Actual vs Predicted)")
plt.legend()
plt.show()
Developed by: 
RegisterNumber:  
*/
```

## Output:
<img width="419" height="286" alt="Screenshot 2026-02-13 142833" src="https://github.com/user-attachments/assets/9c42209a-269b-4fe0-a65c-220d7764e6f9" />
<img width="785" height="576" alt="Screenshot 2026-02-13 142844" src="https://github.com/user-attachments/assets/feac8f92-a316-427f-bc4d-8f45cc51ad80" />



## Result:
Thus the program to implement the multivariate linear regression model for predicting the price of the house and number of occupants in the house with SGD regressor is written and verified using python programming.
