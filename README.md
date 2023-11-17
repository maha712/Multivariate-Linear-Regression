# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1

Import panda

### Step2

Import linear model from sklearn

### Step3

Read the file cars.csv

### Step4

Assign the values for x and y as required

### Step5

Create the linearRegression model and predict the output

## Program:

#To write a python program to implement multivariate linear regression and predict the output.

#program developed by: Mahalakshmi.k

#register number:212222240057

import pandas as pd

from sklearn import linear_model

df=pd.read_csv("/content/cars (1).csv")

x=df[['Weight','Volume']]

y=df['CO2']

regr=linear_model.LinearRegression()

regr.fit(x,y)

print("Coefficient:",regr.coef_)

print("Intercept:",regr.intercept_)

predictedCo2=regr.predict([[300,1300]])

print("Predicted CO@ for the corresponding weight and volume",predictedCo2)


## Output:

![Screenshot (32)](https://github.com/maha712/Multivariate-Linear-Regression/assets/121156360/a0444d66-e443-448a-98b1-8b318ec7c769)

#
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
