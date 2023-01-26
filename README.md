# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import panda

### Step2
import linear mode; from sklearn

### Step3
Read the file cars.csv

### Step4
Assign the values for x and y as required

### Step5
Create the linearRegression model and predict the output

## Program:
```
#Developed by :- M Srinath
#Register number:- 22000990
import pandas as pd
from sklearn import linear_model

df = pd.read_csv('cars.csv')
X = df[['Weight','Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X,y)
print("Cofficients: ",regr.coef_)
print("Intercept: ",regr.intercept_)
predictedCO2 = regr.predict([[3300,1300]])
print('Predicted co2 for the corresponding weight and volume',predictedCO2)







```
## Output:
<img width="802" alt="154982627-b8644868-f27d-4b89-80b0-d887358ff2e4" src="https://user-images.githubusercontent.com/118678482/214790219-41cd16ac-d8d0-4422-a865-5c1c5110d70c.png">


### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
