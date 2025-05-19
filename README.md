# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import Pandas library.
<br>

### Step2
Import Linear_model from sklearn.
<br>

### Step3
Read the csv file using pandas library.
<br>

### Step4
Enter the parameters of the linear function.
<br>

### Step5
Print the parameters of the linear function.
<br>

## Program:
python
~~~
#Program to implement multivariate linear regression and predict the output.
#Developed by: S.SUGESHWA
#Reg no : 21222324230277
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2 = regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)

~~~




## Output:

![WhatsApp Image 2025-05-20 at 00 33 30_07107c94](https://github.com/user-attachments/assets/7674e8ac-0160-4665-a071-7d41ebd4d79c)



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
