# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd.
<br>

### Step2
Read the csv file.
<br>

### Step3
Get the value of x and y variables.
<br>

### Step4
Create the linear regression model and fit
<br>

### Step5
Predict the CO2 emission of a car where the weight is 3300kg and the volume is 1300cm cube.
<br>

### Step6
Print the predicted output
<br>

## Program:
```
\*
# Program to find the multivariate linear regression
# Developed by: V. Yogesh
# Register number: 212223230250
\*
import pandas as pd
from sklearn import linear_model

df=pd.read_csv('cars.csv')
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient",regr.coef_)
print("Intercept",regr.intercept_)
print("Amount",regr.predict([[3300,1300]]))
```
## Output:
![Screenshot 2024-01-02 195815](https://github.com/Yogesh-Yogi-1/Multivariate-Linear-Regression/assets/148514598/b6cdd52f-a607-461a-b38f-bc7b0305372b)
<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
