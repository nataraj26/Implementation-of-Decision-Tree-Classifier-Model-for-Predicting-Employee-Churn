# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the required libraries.

2.Upload and read the dataset.

3.Check for any null values using the isnull() function.

4.From sklearn.tree import DecisionTreeClassifier and use criterion as entropy.

5.Find the accuracy of the model and predict the required values by importing the required module from sklearn.

## Program and Output:
```
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by:NATARAJ KUMARAN S
RegisterNumber:212223230137
```
```
import pandas as pd
from sklearn.preprocessing import LabelEncoder
from sklearn.model_selection import train_test_split
from sklearn.metrics import accuracy_score
from sklearn.tree import DecisionTreeClassifier 
data = pd.read_csv("/content/Employee (1).csv")
data.head()
```
![image](https://github.com/user-attachments/assets/afd5bba9-d2b6-48e1-b801-cb15b1124ab4)

```
data.info()
```
![image](https://github.com/user-attachments/assets/56584e12-23da-4a70-815a-719c2241a25f)

```
data.isnull().sum()
```
![image](https://github.com/user-attachments/assets/f342b0e2-491e-46ad-a603-f96c6e07b54f)

```
data["left"].value_counts()
```
![image](https://github.com/user-attachments/assets/bf0d7f9f-bb93-4122-9aed-9b2f1cb26998)

```
le = LabelEncoder()
data["salary"] = le.fit_transform(data["salary"])
data.head()
```
![image](https://github.com/user-attachments/assets/b658225f-e064-4750-8283-98ad439a1b11)

```
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","promotion_last_5years","salary"]]
x.head()
```
![image](https://github.com/user-attachments/assets/b714f08a-df1e-4271-981b-3ba385d0e8c7)
```
y_pred=dt.predict(x_test)
y_pred
```
![image](https://github.com/user-attachments/assets/57481fca-6410-4c26-924f-7edf349ed7a7)

```
accuracy= accuracy_score(y_test,y_pred)
accuracy
```
![image](https://github.com/user-attachments/assets/1e304346-873e-495e-bba9-29b04db25fa3)



## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
