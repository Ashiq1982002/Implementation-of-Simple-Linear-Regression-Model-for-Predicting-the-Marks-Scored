# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to implement the simple linear regression model for predicting the marks scored.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the standard Libraries.
2. Set variables for assigning dataset values.
3. import linear regression from sklearn.
4. Assign the points for representing in graph.
5. Predict the regression for marks by using the representation of graph.
6. Compare the graphs and hence we obtained the linear regression for the given table.
 

## Program:
```
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: B MUHAMMED ASHIQ 
RegisterNumber:  212220040094
/*
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
dataset = pd.read_csv('student_scores.csv')
dataset.head()
X = dataset.iloc[:,:-1].values
X
Y = dataset.iloc[:,1].values
Y
from sklearn.model_selection import train_test_split
X_train,X_test,Y_train,Y_test = train_test_split(X,Y,test_size = 1/3,random_state = 0)
from sklearn.linear_model import LinearRegression
regressor = LinearRegression()
regressor.fit(X_train,Y_train)
Y_pred = regressor.predict(X_test)
Y_pred
Y_test
plt.scatter(X_train,Y_train,color="blue")
plt.plot(X_train,regressor.predict(X_train),color="brown")
plt.title("Hours vs Scores (Training Set)")
plt.xlabel("Hours")
plt.ylabel("Scores")
plt.show()
plt.scatter(X_test,Y_test,color="blue")
plt.plot(X_train,regressor.predict(X_train),color="brown![Screenshot (10)](https://user-images.githubusercontent.com/93427345/162911172-55fef480-7db3-4d81-b069-feb5782bb30c.png)") 
plt.xlabel("Hours")
plt.ylabel("Scores")
plt.show()
*/
*/
```

## Output:
![sandy](https://user-images.githubusercontent.com/104640895/165984008-bced3eb4-55f7-4cd4-9795-6d5056a96ae0.png)



## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
