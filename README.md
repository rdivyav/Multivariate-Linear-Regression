# Implementation of Multivariate Linear Regression
### Name : Divya R V
### Register Number : 23014030
### Department : CSE(CS)
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas as pd.
### Step2
Read the csv file.
### Step3
Get the value of X and Y variables.
### Step4
Create the linear regression model and fit.
### Step5
Predict the CO2 emission of a car where the weight is 2300kg,and the volume is 1300cm cube.
### Step6
Print the predicted output.

## Program:
### Developed by : Divya R V
### Register Number : 23014030
```
import pandas as pd
from sklearn import linear_model
data= pd.read_csv("cars.csv")
X=data[['Weight','Volume']]
Y=data['CO2']
regr=linear_model.LinearRegression()
regr.fit(X,Y)
print("Coefficient :",regr.coef_)
print("Intercept:",regr.intercept_)
predictCO2=regr.predict([[3300,1300]])
print("prediction CO2 for the corresponding weight and volume",predictCO2)
```
## Output:
![Screenshot 2024-01-02 220817](https://github.com/rdivyav/Multivariate-Linear-Regression/assets/148604723/7f99ca68-8542-44a9-a511-080c2459887b)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
