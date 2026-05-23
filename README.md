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
read the csv file

### Step3
Get the value of x and y variable

### Step4
Create the linear regression model and fit

### Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
input_data = pd.DataFrame({'Weight': [3300], 'Volume': [1300]})
predictedCO2 = regr.predict(input_data)
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)  

```
## Output:
<img width="202" height="164" alt="{98AAD8DF-B250-45E4-99E5-49BD16BE71AB}" src="https://github.com/user-attachments/assets/bba199ee-3b7d-4c91-9f04-ad84e1cc4c17" />
<img width="172" height="82" alt="{EDEC23C6-4096-4B99-925C-4DCB0BAF8837}" src="https://github.com/user-attachments/assets/385730b4-ed9c-473b-ba0f-3aa593977c0e" />
<img width="332" height="50" alt="{77795223-3EC4-4DDE-87C5-3170E69A82E2}" src="https://github.com/user-attachments/assets/553c62ab-1c6d-4b5d-aacb-58ac0ef4ec2c" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
