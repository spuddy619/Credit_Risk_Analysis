# Credit_Risk_Analysis

## Purpose of Analysis
This analysis is meant to see how different methods of supervised machine learning can be used to address unbalanced classification problems. In this instance we are looking to calculate credit risk - a situation in which the number of good loans greatly outnumber the number of risky loans. By employing the use of oversampling, undersampling, and combination, we will create classes of equal sample size from "LoanStats_2019Q1.csv." We will then create two new machine learning models to predict credit risk.

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
  - The balanced accuracy score is around 63% <br/>















