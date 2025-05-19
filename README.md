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
Developed by: T.SANJAI
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
![image](https://github.com/user-attachments/assets/f87f5edf-6bc0-4d46-bd59-da9e6b363ca9)
![image](https://github.com/user-attachments/assets/715b9b46-18e7-43f3-ae2d-32db2d4ba1ff)
![image](https://github.com/user-attachments/assets/6790a961-541e-4c51-87b9-07771e247bdb)
![image](https://github.com/user-attachments/assets/ec9dfdc0-18f9-4662-88f2-1d8462e6a002)
![image](https://github.com/user-attachments/assets/2eaf21a7-d541-483a-b517-d2e28adbe790)
![image](https://github.com/user-attachments/assets/7a75ca41-d757-4f54-aef1-a234d72b9ce5)





## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
