# Credit_Risk_Analysis

## Purpose of Analysis
This analysis is meant to see how different methods of supervised machine learning can be used to address unbalanced classification problems. In this instance we are looking to calculate credit risk - a situation in which the number of good loans greatly outnumber the number of risky loans. By employing the use of oversampling, undersampling, and combination sampling, we will create classes of equal sample size from "LoanStats_2019Q1.csv." We will then create two new machine learning models to predict credit risk.

## Results
### Resampling 
#### Naive Random Oversampling Method
- This method of oversampling creates two equally-sized classes by adding random instances of the minority class until the size of the minority class is equal to that of the majority class.
- Resampling with Random Oversampling seen below: <br/>
![image](https://user-images.githubusercontent.com/72320203/156070381-2d0ec2a6-4955-4f30-8b64-9e9e86b88e4c.png)<br/>
- Training the Logistic Regression model with resampled data: <br/>
![image](https://user-images.githubusercontent.com/72320203/156074568-9bafba1c-dd33-4c29-89ee-9c9b33307bbe.png)<br/>
- Calculate balanced accuracy score: <br/>
![image](https://user-images.githubusercontent.com/72320203/156074650-0f4f9803-f7fd-4f71-ae75-6c399994c6b8.png)<br/>
- Confusion Matrix: <br/>
![image](https://user-images.githubusercontent.com/72320203/156074723-4423001f-fff8-4e69-83b5-34d47e5ca6f1.png)<br/>
- The imbalanced classification report: <br/>
![image](https://user-images.githubusercontent.com/72320203/156074958-f55114e2-808c-4e02-ab6f-06b6416b7ad3.png)<br/>
- Looking at the gathered data we can conclude the following:<br/>
  -Precision <br/>
    - According to the imbalanced classification report, the model's precision in predicting high risk loans is not particulary good at 1% accuracy. <br/>
    - The precision in predicting low risk loans is very accurate at 100% <br/>
  -Balanced Accuracy Score <br/>
    -The balanced accuracy score of this model is around 63% <br/>
#### SMOTE Oversampling
- Resampling data with SMOTE: <br/>
![image](https://user-images.githubusercontent.com/72320203/156084193-8af95061-06f0-4934-b5db-1e9d34827b1b.png) <br/>
- Training Logistic Regression Model with Resampled Data: <br/>
![image](https://user-images.githubusercontent.com/72320203/156084286-1b7c6ac7-1764-4423-971c-7e50ecf7e648.png) <br/>
- Calculate the balanced accuracy score: <br/>
![image](https://user-images.githubusercontent.com/72320203/156084440-2bb4d8f1-9c3d-486c-8971-9b9b60da1dd9.png) <br/>
- Display the confusion matrix: <br/>
![image](https://user-images.githubusercontent.com/72320203/156084505-10ed9cae-ffc9-4248-8291-2ee0e75fd6a7.png) <br/>
- Print the imbalanced classification report: <br/>
![image](https://user-images.githubusercontent.com/72320203/156084602-2bd512ee-9d51-4abd-83eb-997bb5a01de0.png) <br/>


- Looking at the gathered data we can conclude the following:<br/>
  - Precision <br/>
    - This model's precision for high risk loans is 1% <br/>
    - This model's precision for low risk loans is 100% <br/>
  - Balanced Accuracy Score <br/>
    -The balanced accuracy score is around 63% for this model
    
#### Undersampling
- Resampling the data: <br/>
![image](https://user-images.githubusercontent.com/72320203/156085432-6ecc56c9-ae69-4e56-9e46-035ba812cf33.png) <br/>
- Train the Logistic Regression Model using the resampled data: <br/>
![image](https://user-images.githubusercontent.com/72320203/156085621-9b53e4b6-2ce3-4362-91e5-1f99105268c7.png) <br/>
- Calculate the balanced accuracy score: <br/>
![image](https://user-images.githubusercontent.com/72320203/156085705-c2b7f783-73f4-4079-9653-bc794fe9da7a.png) <br/>
- Display the confusion matrix: <br/>
![image](https://user-images.githubusercontent.com/72320203/156085804-8a12bb76-1b8a-46c9-9ee7-97b408c083bf.png) <br/>
- Print the imbalanced classification report: <br/>
![image](https://user-images.githubusercontent.com/72320203/156085888-d92cf6da-0d38-466c-a6cb-4d85fc75d722.png) <br/>

- Looking at the gathered data we can conclude the following:<br/>
  - Precision <br/>
    - This model's precision for high risk loans is 1% <br/>
    - This model's precision for low_risk loans is 100% <br/>
  - Balanced Accuracy Score <br/>
    - The balanced accuracy score for this model is around 63% <br/>

#### Combination (Over and Under) Sampling
- Resample the data: <br/>
![image](https://user-images.githubusercontent.com/72320203/156090462-b8be16b8-bcff-477a-96fb-ec9625e88dd9.png) <br/>
- Train the Logistic Regression Model: <br/>
![image](https://user-images.githubusercontent.com/72320203/156090941-171bbc38-e801-4dea-b6a7-276c8d335402.png) <br/>
- Calculate balanced accuracy score: <br/>
![image](https://user-images.githubusercontent.com/72320203/156097290-824413d8-de45-48bc-8d5a-86813f45a222.png) <br/>
- Display the confusion matrix: <br/>
![image](https://user-images.githubusercontent.com/72320203/156097518-bfaa4d0a-ec8d-4c8e-ba7a-d9b1e854e0b2.png) <br/>
- Print the imbalanced classification report: <br/>
![image](https://user-images.githubusercontent.com/72320203/156097619-d6c563fa-889b-4f84-88a3-b45f856e94bc.png) <br/>

- Looking at the gathered data we can conclude the following: <br/>
  - Precision <br/>
    - This model's precision for high risk loans is 1%
    - This model's precision for low risk loans is 100% 
  - Balanced Accuracy Score <br/>
    - This model's balanced accuracy score is 53% 
  
#### Balanced Random Forest Classifier
- Resample the data: <br/>
![image](https://user-images.githubusercontent.com/72320203/156101536-125bad78-b9ea-41b6-be4c-58a855dff129.png) <br/>
- Calculate the balanced accuracy score: <br/>
![image](https://user-images.githubusercontent.com/72320203/156101864-250407c3-e5d6-4224-b0a9-1bf837eb7bd7.png) <br/>
- Display the confusion matrix: <br/>
![image](https://user-images.githubusercontent.com/72320203/156101985-7bbc214f-4e43-4ee3-9483-1ece725af92f.png) <br/>
- Print the imbalanced classification report: <br/>
![image](https://user-images.githubusercontent.com/72320203/156102076-0302c20e-2be6-418d-8391-6b94e687ff0a.png) <br/>
- List the features sorted in descending order by feature importance: <br/>
![image](https://user-images.githubusercontent.com/72320203/156102155-42de8f54-7d1f-4489-af6c-8b1fb87a7944.png) <br/>

- Looking at the gathered data we can conclude the following: <br/>
  - Precision: <br/>
    - This model has a 4% accuracy for high risk loans <br/>
    - This model has a 100% accuracy for low risk loans <br/>
  - Balanced Accuracy Score <br/>
    - This model has a balanced accuracy score of 79 percent.
#### Easy Ensemble AdaBoost Classifier
- Resample the data: <br/>
![image](https://user-images.githubusercontent.com/72320203/156424772-5c36845e-3c70-40de-ac9e-24ba7deb55c9.png) <br/>
- Calculate the balanced accuracy score: <br/>
![image](https://user-images.githubusercontent.com/72320203/156424951-8e05210f-7da1-42fe-8a62-4db2433a0602.png) <br/>
- Display the confusion matrix: <br/>
![image](https://user-images.githubusercontent.com/72320203/156425054-ef44163d-ab25-474c-a128-54f2c1d7f1bd.png) <br/>
- Print the imbalanced classification report <br/>
![image](https://user-images.githubusercontent.com/72320203/156425152-358ae6c1-b0ca-4b04-ab07-2e188ed7be00.png) <br/>

- Looking at the gathered data:
  - Precision: <br/>
    - This model has a 7% accuracy for high risk loans <br/>
    - This model has a 100% accuracy for low risk loans <br/>
  - Balanced Accuracy Score: <br/>
    - This model has balanced accuracy score of 92 percent <br/>

## Summary
We have concluded that out of the 5 models created and examined, the best model for predicting the high-risk loans was the model that used the Easy Ensemble Adaboost Classifier method; however, the model is not particularly accurate, with a precision of 7% for high risk loans. All the models are excellent at predicting low risk loans but that is not particularly helpful as we want to detect high risk loans. Yes, the Adaboost Classifier is the most precise in this endeavor out of all the models, but with an abysmal precision of 7%. We cannot recommend any of these models for that reason.





  















 




    



















   
   
















