# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

1. .Load employee data and split it into training and testing sets.

2.Train a Decision Tree classifier using entropy as the split criterion.

3.Evaluate the model using accuracy, confusion matrix, and classification report.

4.Use the trained model to predict whether a new employee will stay or leave. 


## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Sushil Shiva R
RegisterNumber: 212224250017
*/
```
```
/*from sklearn.model_selection import train_test_split
from sklearn.tree import DecisionTreeClassifier
from sklearn.metrics import accuracy_score, classification_report, confusion_matrix
df = pd.read_csv("Employee.csv")
df.head()
df.info()
df.isnull().sum()
df.rename(columns={'Departments ': 'Department'}, inplace=True)
df = pd.get_dummies(df, columns=['Department', 'salary'], drop_first=True)
df.head()
X = df.drop('left', axis=1)
y = df['left']
X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42
)
dt_model = DecisionTreeClassifier(
    criterion='gini',
    max_depth=5,
    random_state=42
)
dt_model.fit(X_train, y_train)
y_pred = dt_model.predict(X_test)
accuracy = accuracy_score(y_test, y_pred)
print("Accuracy:", accuracy)
confusion_matrix(y_test, y_pred)
print(classification_report(y_test, y_pred))
from sklearn.tree import plot_tree
import matplotlib.pyplot as plt

plt.figure(figsize=(20,10))
plot_tree(
    dt_model,
    feature_names=X.columns,
    class_names=['Stayed', 'Left'],
    filled=True
)
plt.show()
*/
```
## Output:

<img width="842" height="463" alt="Screenshot 2026-11-02 110048" src="https://github.com/user-attachments/assets/2112cad4-ab58-4a8d-9108-6f50c3a20227" />
<img width="1329" height="687" alt="image" src="https://github.com/user-attachments/assets/b36d4be9-9312-4b00-9dc8-a3660180c268" />




## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
