# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd

### Step2
Read the csv file.

### Step3
Get the value of X and y variables

### Step4
Create the linear regression model and fit

### Step5

Predict the CO2 emission of a car where the weight is 1000kg, and the volume is 1390cm3.

## Program:
```
#Program to Implementation of Multivariate Linear Regression
#Developed by: Suji.G
#Register number: 22008563
import pandas as pd
from sklearn import linear_model

df = pd.read_csv("cars.csv")

X = df[['Weight', 'Volume']]
y = df['CO2']

regr = linear_model.LinearRegression()
regr.fit(X, y)

print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)

predictedCO2 = regr.predict([[1000, 1390]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)





```
## Output:

![pppp](https://user-images.githubusercontent.com/119559822/214363482-6c3d2af0-aa88-43bc-88bd-adaf6b1f07b8.png)
![pp](https://user-images.githubusercontent.com/119559822/214363522-52e3b57f-d8fa-460d-8df6-5015d7d95fed.png)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
