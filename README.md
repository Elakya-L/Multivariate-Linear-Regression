# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import the required libraries such as pandas and sklearn for data handling and regression.

### Step2
Load the dataset from the CSV file using pandas.

### Step3
Separate the independent variables (Volume, Weight) as input (X) and dependent variable (CO2) as output (y).

### Step4
Create a Linear Regression model and fit the model using the training data.

### Step5
Print the coefficients, intercept, and predict the output for given input values.

## Program:
```
#Regsiter number: 21222523006
#Developed by: Elakya L

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car (1).csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[3300,1300]]))

```
## Output:

![alt text](<WhatsApp Image 2026-03-17 at 11.05.36 AM.jpeg>)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.