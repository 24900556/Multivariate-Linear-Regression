# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas as pd

### Step2
Read the csv file

### Step3
Get the value X and Y variables
### Step4
Create the linear regression model and fit

### Step5
Predict the c02 emission of a car where weight is 2300 kg, and the volume is 1300cm
cube and print the output.



## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car.csv")

df.info()

df.head()

df.tail()

x=df[['Weight', 'Volume']]

y=df['CO2']

regr=linear_model.LinearRegression()

regr.fit(x,y)

print('Coeffients:',regr.coef_)

print('Intercept:',regr.intercept_)

predictedCO2=regr.predict([[3300,1300]])

print('Predicted CO2 for the corresponding weight and volume', predictedCO2)





```
## Output:

### Insert your output
![alt text](<Screenshot 2024-12-31 071822.png>)


<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.