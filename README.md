# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the necessary packages using import statement.
2. Read the given csv file and print the number of contents to be displayed.
3. Split the dataset using train_test_split.
4. Calculate Y_Pred and accuracy.
5. Display the result. 

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: LALITHA PARAMESWARI.C
RegisterNumber:  212219220027
import pandas as pd
data=pd.read_csv("spam.csv",encoding='latin-1')
data.head()
data.info()
data.isnull().sum()
x=data["EmailText"].values
y=data["Label"].values
from sklearn.model_selection import train_test_split 
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)
from sklearn.feature_extraction.text import CountVectorizer
cv=CountVectorizer()
x_train=cv.fit_transform(x_train)
x_test=cv.transform(x_test)
from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)
y_pred=svc.predict(x_test)
y_pred
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
*/
```

## Output:
## Data.head():

![image](https://user-images.githubusercontent.com/103946827/174739027-865d9b63-3c9f-4e62-85df-775dad0b7c14.png)

## Data.info():

![image](https://user-images.githubusercontent.com/103946827/174739123-6f74fdb6-a262-433b-9a4d-d542a40ed7e7.png)

## Data.isnull().sum():

![image](https://user-images.githubusercontent.com/103946827/174739263-90a01488-f729-4210-879a-68fbfc3de0c7.png)

## Y_Pred:

![image](https://user-images.githubusercontent.com/103946827/174739379-342748b1-a4bc-4ca9-9967-f2437be23bc7.png)

## Accuracy:

![image](https://user-images.githubusercontent.com/103946827/174739449-66dae239-d1dd-431a-b524-56ff1c5bd503.png)



## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
