# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the packages.

2.Analyse the data.

3.Use modelselection and Countvectorizer to preditct the values.

4.Find the accuracy and display the result.
## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: SANJAI.T
RegisterNumber: 24900899
import pandas as pd
data=pd.read_csv("spam.csv", encoding='Windows-1252')
data

data.shape

x=data['v2'].values
y=data['v1'].values
x.shape

y.shape

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.2, random_state=0)
x_train

x_train.shape
from sklearn.feature_extraction.text import CountVectorizer
cv=CountVectorizer()
x_train=cv.fit_transform(x_train)
x_test=cv.transform(x_test)
from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)
y_pred=svc.predict(x_test)
y_pred

from sklearn.metrics import accuracy_score,confusion_matrix,classification_report
acc=accuracy_score(y_test,y_pred)
acc

con=confusion_matrix(y_test,y_pred)
print(con)

cl=classification_report(y_test,y_pred)
print(cl)
*/
```

## Output:
### data
![image](https://github.com/user-attachments/assets/037077e1-62f6-4059-9021-2fb70618c799)
### data.shape()
![image](https://github.com/user-attachments/assets/a17af88f-5b08-4e02-a26c-0f21c068caa5)
### X.shape()
![image](https://github.com/user-attachments/assets/fe0819ca-8cea-4bd6-b248-c3e5b85a120b)
### y.shape()
![image](https://github.com/user-attachments/assets/1f8b531a-e9bd-49a2-8177-1e821d20471d)
##3 x_train
![image](https://github.com/user-attachments/assets/c558e5d3-5370-47a6-aebd-f2d36bce6011)
### x_train.shape()
![image](https://github.com/user-attachments/assets/06cd3265-3a64-44d0-850f-ac7ac49d19da)
### y_pred
![image](https://github.com/user-attachments/assets/e2a6be75-f682-49dc-b924-56a997961971)
### acc(accuracy)
![image](https://github.com/user-attachments/assets/0389a12c-f83b-442d-9168-8428dfeb17d0)
### con(cofusion matrix)
![image](https://github.com/user-attachments/assets/320a87bc-f877-485d-aa9c-e35e53b5aeec)
### cl(classification report)
![image](https://github.com/user-attachments/assets/87956628-cc01-41e3-bc13-aa0cdef05422)




## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
