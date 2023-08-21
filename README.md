# EXP-3-Implementation-of-log-transformation

## AIM:
Perform log transformation on international airline passenger data.
## ALGORITHM:
### STEP 1: Import the required packages like pandas and numpy
### STEP 2: Read the data using the pandas
### STEP 3: Perform the data preprocessing if needed and apply log transformation.
### STEP 4: Plot the data according to need, before and after log transformation.
### STEP 5: Display the overall results.

## PROGRAM:
```
import numpy as np
import pandas as pd
data= pd.read_csv('AirPassengers.csv')
data.head()
data.dropna(inplace=True)
x=data['Month']
y=data['#Passengers']
data_log=np.log(data['#Passengers'])
X=data['Month']
Y=data_log
import matplotlib.pyplot as plt
plt.plot(x,y)
plt.xlabel('Original Data')
plt.plot(X,Y)
plt.xlabel('Log- Transformed data')
```
## OUTPUT:
### FIRST FIVE ROWS:
![image](https://github.com/gpavithra673/EXP-3-Implementation-of-log-transformation-/assets/93427264/dee7e959-a649-4ac3-905c-985d80f92346)

### BEFORE LOG TRANSFORMATION:
![image](https://github.com/gpavithra673/EXP-3-Implementation-of-log-transformation-/assets/93427264/31b5cfdd-8787-4957-8f2c-07e409d43762)
### AFTER LOG TRANSFORMATION:
![image](https://github.com/gpavithra673/EXP-3-Implementation-of-log-transformation-/assets/93427264/c45837a1-4334-41a6-8731-bd1de76d9a1c)

## RESULT:
### Thus we have created the python code for the log transformation on international airline passenger data.
