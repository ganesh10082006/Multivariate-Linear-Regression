# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Read the csv file.
### Step2
Get the value of X and y variables
### Step3
Create the linear regression model and fit.
### Step4
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.
### Step5
Print the predicted output.
## Program:
```
Developed by: GANESH G.
Reg.No: 212223230059

import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
Y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, Y)
print('Coefficients:', regr.coef_)
print('Intercept:',regr.coef_)
predictedCO2 = regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding Weight and Volume',predictedCO2)

```
## Output:

### Insert your output
![image](https://github.com/ganesh10082006/Multivariate-Linear-Regression/assets/151981672/b0925429-f92b-4ab7-9f79-64b6d4fb973c)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
