# Credit_Risk_Analysis

## Overview of the Project
<p align="justify">The purpose of this projects was to evaluate different machine learning models to determine which of them performs better when it comes to making a credit risk analysis. </p>
<p align="justify">This project was performed in Jupyter Notebook using different libraries like pandas and sklearn. </p>

## Results
In order to make a credit risk analysis 6 distinct models were used. In this section the 6 models will be evaluated regarding their balanced accuracy scores and the precision and recall scores.

1.	Naive Random Oversampling 

•	The balanced accuracy score for this model was 0.61, which is not a high number. This model is not the best at determining the loan status.

•	The precision in which the model classifies the high-risk loan status is very low. This could mean that a lot of false positives can be expected when using this model. 

•	The recall is low in both high and low risk loan status. Although is not very low, it would not be advisable to use this model because it would show a significant number of false negatives


<img width="337" alt="1" src="https://user-images.githubusercontent.com/111388644/212773976-0dbbeb57-8201-4aaa-bffd-d9bebf8faa8d.png">

<img width="486" alt="2" src="https://user-images.githubusercontent.com/111388644/212774000-39955394-c2a3-4616-8ac2-e3a998cac0a4.png">


2.	SMOTE Oversampling

•	The balanced accuracy score in this model is 0.62, which is very similar to the previous one. This also means that the models accuracy is not as high as desired in order to classify the high and low risk loans correctly. 

•	The precision has the same problem than the last model. It is very low for the high-risk loans: 0.01

•	The recall also happens to be somewhat low, although is it better than the precision. The recall is: 0.59 and 0.66


<img width="281" alt="3" src="https://user-images.githubusercontent.com/111388644/212774033-eed3d8b8-b281-4365-85e1-e9742ace849b.png">

<img width="525" alt="4" src="https://user-images.githubusercontent.com/111388644/212774058-739b000c-6e00-44e6-8d52-b410656f2b34.png">


3.	Undersampling

•	The accuracy score of the undersampling model was very low. It had a score of 0.50. It is even lower than the accuracy scores of the SMOTE and the Naïve Random Oversampling models

•	The precision had a value of 0.99 for the low-risk loans and 0.01 for the high-risk ones. Even though the score for the low risk one is almost 1, the other score is too low.



•	The two values for the recall regarding the high and low risk were 0.59 and 0.43 respectively. These scores are not good enough for the model to asses the risk when it comes to loans. 

<img width="341" alt="5" src="https://user-images.githubusercontent.com/111388644/212774088-4ab7e6d5-53e2-467b-a346-ace3129aab5e.png">

<img width="492" alt="6" src="https://user-images.githubusercontent.com/111388644/212774109-a3af163f-8795-4fb6-99a1-0f43a998268c.png">


4.	Combination (Over and Under) Sampling

•	The accuracy score in this model had a value of 0.64, which means that it is 64% accurate. It may not be accurate enough. 

•	The precision score was great in the low-risk evaluation. On the other hand, the precision for the high-risk loans is very poor. 

•	The values of the recall were 0.72 and 0.57. The first one refers to the high-risk loans. This means that when it comes to detecting those type of loans this model is better than the other 3 above. 


<img width="329" alt="7" src="https://user-images.githubusercontent.com/111388644/212774132-7ab1007d-f695-4925-8a24-33a382e21836.png">

<img width="503" alt="8" src="https://user-images.githubusercontent.com/111388644/212774169-52d369d8-434a-444a-ab86-13a610670774.png">


5.	Balanced Random Forest Classifier

•	The accuracy of this model is slightly better than the other 4 models. The value of the accuracy score was 0.78. This means that the model is 78% accurate. 

•	The precision did not improve much when it comes to the high-risk loans since it has a value of 0.04.

•	In this model there were 64% of true positives found for the high-risk loans, and 92% for the low-risk ones.


<img width="444" alt="9" src="https://user-images.githubusercontent.com/111388644/212774186-3692b1cf-b83f-4b41-affa-100e1f9d68e0.png">

<img width="484" alt="10" src="https://user-images.githubusercontent.com/111388644/212774202-59d1fd12-37f8-41ca-806b-a41b1854bbd9.png">


6.	Easy Ensemble AdaBoost Classifier

•	The accuracy score for this model is impressive since it is 93% accurate. This model is superior to all the other ones that were reviewed. 

•	The precision improved very little in the high-risk loans, but it is better in the low risk-ones. But on average it has a value of 0.99.

•	The recall is very good in both scores. The model identifies the true positives in an amazing way.


<img width="374" alt="11" src="https://user-images.githubusercontent.com/111388644/212774227-d3b01271-5e14-4a00-9d05-afc703322d5c.png">

<img width="493" alt="12" src="https://user-images.githubusercontent.com/111388644/212774247-38106a15-0ef7-44b7-b215-33546a23bd81.png">



## Summary
<p align="justify">Out of the 6 models the one that performed the best was the Easy Ensemble AdaBoost Classifier. This would be the advised model to use since it has a high accuracy score ass well as recall.</p>

<p align="justify">The other ones would not be as recommended since the accuracy is low, and the recall does not indicate a high percentage of identifying the true positives. This means that the other 5 models may fail to point out important information.</p> 
