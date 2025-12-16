# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

Hardware – PCs
Anaconda – Python 3.7 Installation / Jupyter notebook 

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: vignesh s
RegisterNumber: 25014344 
*/
import pandas as pd

from IPython.display import display

data = pd.read_csv("Employee.csv")

print("===== DATA HEAD (5 ROWS) =====")

display(data.head())

print("\n===== DATA INFO =====")

print(data.info())

print("\n===== MISSING VALUES =====")

display(data.isnull().sum().to_frame("Missing Values"))

from sklearn.preprocessing import LabelEncoder

le = LabelEncoder()

data["salary"] = le.fit_transform(data["salary"])

print("\n===== X HEAD (5 ROWS) =====")

display(x.head())

from sklearn.model_selection import train_test_split

x_train, x_test, y_train, y_test = train_test_split( x, y, test_size=0.2, random_state=100 )

from sklearn.tree import DecisionTreeClassifier

dt = DecisionTreeClassifier(criterion="entropy")

dt.fit(x_train, y_train)

y_pred = dt.predict(x_test)

rom sklearn import metrics

accuracy = metrics.accuracy_score(y_test, y_pred)

print("\n===== MODEL ACCURACY =====")

print("Accuracy:", accuracy

```

## Output:

<img width="920" height="183" alt="Screenshot 2025-12-16 110418" src="https://github.com/user-attachments/assets/159e73c1-9eb6-49a0-a76a-9b3503df5246" />

<img width="643" height="458" alt="Screenshot 2025-12-16 110423" src="https://github.com/user-attachments/assets/e30c1bfc-87ef-4767-97e7-945090c0fa4b" />

<img width="515" height="75" alt="Screenshot 2025-12-16 110435" src="https://github.com/user-attachments/assets/032c26aa-4a06-4af8-a54e-f36548b2795f" />

<img width="471" height="471" alt="Screenshot 2025-12-16 110428" src="https://github.com/user-attachments/assets/82a4ce8b-c861-4052-896c-2a2276f8cf0c" />


<img width="908" height="184" alt="Screenshot 2025-12-16 110439" src="https://github.com/user-attachments/assets/047eea8b-2f9c-47cc-9752-77a012d7c823" />

<img width="916" height="182" alt="Screenshot 2025-12-16 110445" src="https://github.com/user-attachments/assets/50d78c7b-0646-440b-8809-c98d1a9f0901" />

<img width="422" height="152" alt="Screenshot 2025-12-16 110451" src="https://github.com/user-attachments/assets/8437ca0d-bcc6-4d41-9a34-0471089d9c48" />


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
