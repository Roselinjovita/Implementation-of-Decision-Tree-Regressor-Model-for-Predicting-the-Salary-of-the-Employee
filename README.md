# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the libraries and read the data frame using pandas.

2. Calculate the null values present in the dataset and apply label encoder.

3. Determine test and training data set and apply decison tree regression in dataset.

4. Calculate Mean square error,data prediction and r2.
   
## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: S.ROSELIN MARY JOVITA
RegisterNumber:  212222230122

import pandas as pd
data=pd.read_csv("/content/Salary.csv")

data.head()

data.info()

data.isnull().sum()

from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()

x=data[["Position","Level"]]
y=data["Salary"]

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)


from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)

from sklearn import metrics
mse=metrics.mean_squared_error(y_test,y_pred)
mse

r2=metrics.r2_score(y_test,y_pred)
r2

dt.predict([[5,6]])
  
*/
```


## Output:
#  data.head()

![Screenshot 2023-10-14 211306](https://github.com/Roselinjovita/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119104296/68bd816e-72b2-462e-ab46-8ef4613e47bb)

# data.info()

![Screenshot 2023-10-14 211314](https://github.com/Roselinjovita/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119104296/851341dc-3d59-447d-88c2-d856d2c24e91)

# isnull() and sum()

![Screenshot 2023-10-14 211320](https://github.com/Roselinjovita/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119104296/2a2defde-170f-460b-9b9e-31ae97459493)

# data.head()  for salary

![Screenshot 2023-10-14 211327](https://github.com/Roselinjovita/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119104296/620e4b39-976f-4c16-a707-90c28a96e90b)

# MSE value

![Screenshot 2023-10-14 211338](https://github.com/Roselinjovita/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119104296/d1534d15-83f6-4518-a07b-352282841664)

# r2 value
![Screenshot 2023-10-14 211342](https://github.com/Roselinjovita/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119104296/9fd5e6b9-e13c-496b-99da-a01d1353c18a)

# data prediction

![Screenshot 2023-10-14 211355](https://github.com/Roselinjovita/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/119104296/5f038b03-8884-431c-8d92-6aa1d82d1664)



## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
