# Logistic_Regression_Heart_Attack_Prediction

# Purpose 
Gain experience outside of online courses and tutorials with Logistic regression and interpreting results. 

# Methods 
Using SKlearn logistic regression function and a dataset from Kaggle to predict heart attacks. Focused on subset of attributes with highest correlation to heart attacks in the data set. 

CP - chest pain, 
thalach - max heart rate,
exang - exercise induced angina,
slope = slope of peak excercise ST segment (of ECG),
old peak = ST depression induced by exercise relative to rest 

# Results 
Looked at correlation between heart attack and the 14 attributes in the dataset. Created a simplier model to focus on the attributes listed in the methods section. This yielded slightly better results and keeps the model simple. The results of the model are displayed in the confusion matrix below.

![image](https://user-images.githubusercontent.com/35962729/120228166-9503f400-c218-11eb-8dee-d0a1c688937d.png)

The results are also displayed as area under the curve with a AUC of 0.86. The AUC uses a combination of the true positive rate (recall) and false positive rate). We would expect a random model to have 0.5 AUC. 
![image](https://user-images.githubusercontent.com/35962729/120228595-73573c80-c219-11eb-838f-c7db055a7092.png)



# Learnings 
For predicting heart attacks we would ideally like to limit the amount of type 2 errors (False Negative). Meaning that we predicted no heart attack when there was a heart attack. For medical applications, it would be better to bias the error towards false positive then run additional tests to confirm. To bias this we could raise/lower the threshold of the logistic regression. 
