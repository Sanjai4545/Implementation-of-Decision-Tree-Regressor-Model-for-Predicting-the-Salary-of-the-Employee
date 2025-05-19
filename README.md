# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import pandas
2.Import Decision tree regressor
3.Fit the data in the model
4.Find the accuracy score

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: SANJAI.T
RegisterNumber:  24900899
import pandas as pd
df=pd.read_csv("/content/Salary.csv")
df.head()
df.info()
df.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
df["Position"]=le.fit_transform(df["Position"])
df.head()
x=df[['Position','Level']]
x.head()
y=df['Salary']
y.head()
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
y_pred
from sklearn.metrics import r2_score
r2=r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])
*/
```

## Output:
![WhatsApp Image 2025-05-19 at 10 08 27_b7b38d56](https://github.com/user-attachments/assets/e5db4f3c-ebf4-4525-a55b-98bfb16901cc)
![WhatsApp Image 2025-05-19 at 10 08 27_ce5e2a7c](https://github.com/user-attachments/assets/df55d377-a207-414b-a5a0-f608d8d8e0a7)
![WhatsApp Image 2025-05-19 at 10 08 27_ce93b913](https://github.com/user-attachments/assets/ed14feb4-e250-4483-a5a9-0ffd44743352)
![WhatsApp Image 2025-05-19 at 10 08 27_a9e70c10](https://github.com/user-attachments/assets/0aa06496-bcc8-4b08-aba8-8f976fa03276)
![WhatsApp Image 2025-05-19 at 10 08 27_68225b9c](https://github.com/user-attachments/assets/f9265d85-fbc8-4a0b-87f1-67e3a8ee4040)


## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
