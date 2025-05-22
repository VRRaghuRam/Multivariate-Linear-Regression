# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import necessary libraries like pandas and sklearn.linear_model.

### Step2
Read the dataset using pandas.read_csv() and extract input (Volume, Weight) and output (CO2) variables.

### Step3
Initialize a Linear Regression model using LinearRegression().

### Step4
Train the model using the .fit(x, y) method.

### Step5
Predict the output for new input data using .predict().

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car (1).csv")
x=df[["Volume","Weight"]]
y=df[["CO2"]]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[3300,1300]]))

```
## Output:

![alt text](<Screenshot (68).png>)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.