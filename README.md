# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the required libraries.
2.Upload and read the dataset.
3.Check for any null values using the isnull() function.
4.From sklearn.tree import DecisionTreeClassifier and use criterion as entropy.
5.Find the accuracy of the model and predict the required values by importing the required module from sklearn.
  

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: V.Divyashree
RegisterNumber:  212223230051

import pandas as pd
data=pd.read_csv("Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x=data[["satisfaction_level","last_evalution","number_project","average_montly_hours","time_spend_company","work_accident","promotion_last_5years","salary"]]
x.head()
y=data["left"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
dt.predict([[0.5,0.8,9,260,6,0,1,2]])


*/
```

## Output:
Data.head():

![image](https://github.com/divya280/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/82276099/23f56b0d-4809-4663-9077-3a398dbdedc2)

Data.info():

![image](https://github.com/divya280/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/82276099/5ce69f4c-ee4b-4d05-b796-ba454de84c10)

isnull() and sum():

![image](https://github.com/divya280/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/82276099/b12806c5-1148-4286-8c05-8c72391e3788)

Data Value Counts():

![image](https://github.com/divya280/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/82276099/cea7c29b-79cf-4d55-96dd-cb13c04cab03)

Data.head() for salary:

![image](https://github.com/divya280/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/82276099/bb02d74e-0883-4dcf-941c-757c622f40e6)

x.head:

![image](https://github.com/divya280/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/82276099/54d0b2a5-c026-4df0-99d4-6426c50aa643)

Accuracy Value:

![image](https://github.com/divya280/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/82276099/bc61df76-5f7f-49b8-bd84-1da796781868)

Data Prediction:

![image](https://github.com/divya280/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/82276099/4e060bc8-0938-46da-8e1a-2cdc97ff6501)



## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
