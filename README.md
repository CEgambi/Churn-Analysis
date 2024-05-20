# CUSTOMER CHURN ANALYSIS - SyriaTel 

![image](https://daxg39y63pxwu.cloudfront.net/images/blog/churn-models/Customer_Churn_Prediction_Models_in_Machine_Learning.png)


## Author

[Charles Egambi]



## Overview

SyriaTel is a telecommunications company in Syria. They have been informed that some of their customers have started to churn, discontinue their service. This analysis will determine what features will indicate if a customer will ("soon") discontinue their service.

## Business Problem

In the highly competitive telecom industry, customer churn represents a critical challenge that directly impacts profitability and market share. The dataset under analysis offers essential insights into customer behavior, helping to identify the key factors influencing churn. By utilizing predictive analytics, telecom companies can proactively mitigate customer attrition, thereby optimizing retention strategies and improving overall business performance.


## Data

In this report, a dataset on churn data of a Telecom company is analysed. It can be found here: 'https://www.kaggle.com/becksddf/churn-in-telecoms-dataset'.

## Methods

1. Data preparation was conducted including the identification and handling:
    - Missing values
    -  Duplicates
    - Outliers
    - Data types for specific variables
The original data set contained 3,333 rows of data. After Data preparation, a total of 3,169 rows were adopted for further analysis. 
The following Churn features were used in conducting the analysis: state, account length, area code, phone number, international plan, voice mail plan, number vmail messages, total day minutes, total day calls, total day charge, total eve minutes, total eve calls, total eve charge, total night minutes, total night calls, total night charge, total intl minutes, total intl calls, total intl charge, customer service calls, churn.
2. Exploratory Data Analysis
 EDA was conducted  by:
    -  assesing descriptive statistics of the dataset
    - visualizing outputs in Barcharts, Histograms, scatterplots and Heatmap to understand the distribution and correlation of various features.
3. Modelling
   - Logistic Regression
   - Random Forest
   - Decision Tree
     - Feature Engineering
     - One Hot Encoding(Dealing with categorical Data)
     - Normalization/Standadization
     - Split- Train Test
     - Model Evaluation

## Results


### Logistic Regression Model:

According to the logistic regression classifier model, total day charge, number of voicemail messages and total evening charge are the top three important features.
Model accuracy is 76.5%, which is not bad. F1 score is only 50.2% which means the test will only be accurate half the times it is run.

Accuracy score for testing set:  0.76545
F1 score for testing set:  0.50267
Recall score for testing set:  0.72868
Precision score for testing set:  0.38367

### Random Forest Model:

According to the random forest classifier; 'total day charge', 'customer service calls' and 'international plan' features have the highest impact on the model.
Accuracy and F1 score are much higher than the Logistics Regression Model

Accuracy score for testing set:  0.92182
F1 score for testing set:  0.75
Recall score for testing set:  0.72093
Precision score for testing set:  0.78151

### Decision Tree Model:

According to the decision tree Model, 'customer service calls', 'total day charge' and 'total evening charge' are the three most important for the model.
The accuracy and F1 score for this model is lower than the Random Forest Model

Accuracy score for testing set:  0.88525
F1 score for testing set:  0.67616
Recall score for testing set:  0.73643
Precision score for testing set:  0.625

## Conclusion

Tree Model performed well on our dataset compared to the Random Forest Model and Logistic Regression Model.

## Recommendation

Based on the findings, it is recommended to focus on the Decision Tree Model for predicting customer churn in the telecom sector. This model has shown superior performance on the dataset. While the Random Forest and the Logistic regression did not perform as well, further exploration into advanced feature engineering and threshold adjustments could potentially enhance their effectiveness.