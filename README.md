# IBM-HR-employee-Attrition-Prediction-
![image](https://github.com/Poojamotekar/IBM-HR-Analytics-Employee-Attrition-Performance/assets/66488693/2c27241e-dbb0-4c00-ad66-3a3eecf66c67)

![image](https://github.com/Poojamotekar/IBM-HR-Analytics-Employee-Attrition-Performance/assets/66488693/770b5b07-abfc-4ce8-9b85-36497106f2d3)

## Dataset source
- https://www.kaggle.com/pavansubhasht/ibm-hr-analytics-attrition-dataset

*In this project, we perform a complete machine learning work flow from data exploratory and feature engineering to build different machine learning models and evaluate model performances to predict if an employee will leave his/her current employer and analyze what features will mainly affect employee's attrition activity.*

# Contents of the project
  
  1. Data Exporatory and analysis

  2. Feature engineering

  3. Model training and performance evaluations

  4. Feature importance analysis

## Data Exporatory and analysis

*Data exporatory is the most important part of the work flow for machine learning project as it is the first approach to understand the whole dataset and all the features including numerical and non numerical, missing data, duplicate data, meaningful and meaningless. Since we will try the best to understand and apply all the useful features to the models later on, we would have to make ourself understand all the features that we have.*

### Visualization
*It is one of the most effective ways to understand the statistical distribution and detect potential outliers in our dataset.*

#### Distribution of Target Variable
![image](https://github.com/Poojamotekar/IBM-HR-Analytics-Employee-Attrition-Performance/assets/66488693/f95e6e71-7f89-46f0-b293-296c586aab43)
 
 As we could see the distribution of our target variable is **imbalanced** for the binary variable yes and no.

#### Distribution of Numerical Features 
![image](https://github.com/Poojamotekar/IBM-HR-Analytics-Employee-Attrition-Performance/assets/66488693/504cd43c-51ea-4711-9be7-58fe1fee627d)

This is the distribution of our numerical features. We have preprocessed all the numerical features so there are no missing data or duplicate data. 
From the exproratory, it looks like exit employee's **age** and **working time with his current position** give out some signals of attrition as well as **dailyrate** which refers to paystub.

#### Distribution of Non Numerical Features
![image](https://github.com/Poojamotekar/IBM-HR-Analytics-Employee-Attrition-Performance/assets/66488693/9cfd0876-1c58-44e0-881b-1fadb175deee)

This is the distribution of non numerical features. Even though all the distribution is imbalanced, we could still tell that too much **over time** work definitely will drive away a loyal employee. **Traveling** and **martial status** will also be considered as factors of the effect.

## Feature Engineering

#### Correlation Matrix

From this matrix we could be able to see correlations between each feature and between features and target variable. For correlation score > 0.5, we would consider the two features are correlated.

*For non numerical features, we applied one hot encoding and transform them into numerical.*

## Model Training


## Model Evaluation

*There are different metrics to evalutate a model's performance. For classification problem, which is what we tried to solve in this project, accuracy is one of the metric that we will look at. Beside accuracy, precision and recall is another metric that we need to pay more attention especially for imbalanced variable. Assuming we only have 1 employee exit in our dataset and we predict everyone is staying, then we will have a model with accuracy 99% which still cannot be able to help us to find out the employee who would like to exit. So precision recall and f1 score will the metric for our evaluation. And to better evaluate and visualize the result of precision and recell, we use confusion matrix graph with labels of acutal and prediction.*
![image](https://github.com/Poojamotekar/IBM-HR-Analytics-Employee-Attrition-Performance/assets/66488693/7ea5af15-3002-474a-8971-d0881dd7b4f8)  ![image](https://github.com/Poojamotekar/IBM-HR-Analytics-Employee-Attrition-Performance/assets/66488693/4eeeb2ea-0a3c-4f54-bc03-8af54163a015)



 ![image](https://github.com/Poojamotekar/IBM-HR-Analytics-Employee-Attrition-Performance/assets/66488693/1571c9ba-5873-4807-a7ac-9425a63e704e) ![image](https://github.com/Poojamotekar/IBM-HR-Analytics-Employee-Attrition-Performance/assets/66488693/8368bc4e-ff75-4707-b03b-d566b0b0f999)



## Feature Importance

*This is the most important analysis that gained from random forest and LASSO aka linear model with regularization. The feature importance reveals how important each feature is and how it will affect the performance of the model.*

![image](https://github.com/Poojamotekar/IBM-HR-Analytics-Employee-Attrition-Performance/assets/66488693/4a4d4801-3408-4707-bc6c-6a158c65a903)


## Conclusions

*It is quite obvious and it is a conclusion that everyone will accept, which is paying more and working less may be the eltimate dream for all employees.
Overtime, monthlyrate, age, years of works they all are very important feature that will affect the attrition activity and performance of an employee. So it will be quite efficient to apprach to those higher risk employees and better communicate with them, so that their intention of attrition could be resolved. It will be beneficial for both employer and employee. Otherwise, plan ahead of time to hire new candidate will be an alternative option.*

## Future Plans and Works

*This is a complete flow for machine learning and there is still much of work to do. We will need to spend more time on tuning the model so that we will have a more robust model that could be deployed in the future. If possible, we could collect more data and more feaetures so that the model could learn more from data and make more accurate predictions.*
