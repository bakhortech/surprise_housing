# Project Name
#### Surprise Housing Assignment


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)


## General Information
A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file train.csv.

The company is looking at prospective properties to buy to enter the market. Objective is to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

The company wants to know:

    Which variables are significant in predicting the price of a house, and

    How well those variables describe the price of a house.

 

Also, the optimal value of lambda for ridge and lasso regression needs to be determined.

## Conclusions
- Exploratory analysis was done on the dataset based on continuous and categorical variables.
- There were columns with more than 40% null values. Those are dropped from the dataset.
- There were also some skewed columns. The highly skewed columns are dropped and moderatly skewed columns are adjusted by combining minority columns into one column.
- Null or empty values are replaces with median for columns having outliers and mean for other continuous variables.
- The best model out of 5 fold cross validated model using Ridge and Lasso regularization has been chosen as final model. This shows the best model out of the available training set.
- The optimal value of alpha for ridge regression is 10 and for Lasso regression is 0.00006.
- Top 5 features using Ridge regression are:

      - 'SaleCondition_Others', 0.057
      - 'GarageFinish_RFn', 0.052
      - 'GarageFinish_Unf', 0.052
      - 'SaleCondition_Normal', 0.052
      - 'GarageFinish_No Garage', 0.048
- Top 5 features using Lasso regression are:

      - ('GarageFinish_No Garage', 0.051)
      - ('GarageFinish_RFn', 0.066)
      - ('GarageFinish_Unf', 0.072)
      - ('SaleCondition_Normal', 0.074)
      - ('SaleCondition_Others', 0.302)
- A decent score for Ridge and Lasso Regression were observed which are as follows-
    Ridge Regression Score:
    
            Train Score : 0.9048825126844456
            Test Score : 0.8762875068524612
    Lasso Regression Score:
    
            Train Score : 0.9178195810624109
            Test Score : 0.883834546544181
- The values of train and test score are very near which shows the model is properly fit on the data and is supposed to predict target values with higher confidence.
- On plotting mean test and train scores with alpha we could observe similar curve for both train and test data. 
## Technologies Used
- jupyter notebook - version 6.0.3
- python - version 3.8
- pandas - version 1.0.5
- numpy - version 1.18.5
- matplotlib.pyplot
- seaborn - version 0.10.1
- sklearn

## Acknowledgements
This project is created as part of upgrad assignment on linear regression. Thanks to upgrad for inspiring to work on interesting problems.

## Contact
Created by [@bakhortechnologies] - feel free to contact me!