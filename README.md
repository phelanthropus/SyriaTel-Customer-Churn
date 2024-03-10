# SyriaTel Customer Churn #

## Introduction ##
In the competitive landscape of telecommunications, retaining existing customers has become paramount for sustained growth and profitability. With Syriatel Mobile Telecom, a leading provider  the's telecommunications sector, facing the challenge of customer churn, there arises a critical need to implement proactive measures to identify and retain customers at risk of churn. This project aims to leverage machine learning techniques to predict customer churn and subsequently inform retention strategies, thereby safeguarding Syriatel's market position and fostering long-term growth.

## Business Understanding ##

### Problem Statement ###
The primary objective is to develop a classifier model that predicts whether a customer is likely to churn, allowing Syriatel to intervene with targeted retention strategies. Customer churn, defined as the discontinuation of services by subscribers, poses a significant threat to revenue streams and market position. By identifying patterns in customer behavior and demographic data, Syriatel seeks to mitigate the financial impact of churn and uphold customer satisfaction.

### Stakeholders ###
Syriatel Mobile Telecom stands as the principal stakeholder, driven by the imperative to reduce churn rates and bolster profitability. Additionally, shareholders, employees, and customers all have vested interests in the company's success. Through customer retention initiatives, the company aims to enhance customer experience, increase shareholder value, and foster employee satisfaction.

### Objectives and Research Questions ###

- Identify key features influencing churn prediction.
- Determine optimal machine learning models for churn prediction.
- Devise customer retention strategies to minimize churn rates.

### Dataset Overview ###
The dataset, sourced from Kaggle, comprises 3333 entries and 21 columns detailing customer activity and churn status. Key features include account length, international plan status, call statistics, and customer service interactions. Exploratory data analysis will uncover insights into data quality and potential predictors of churn.

### Data Preparation

The initial phase of the analysis involved a thorough data preparation process encompassing the following key steps:
1. Data Cleaning: The dataset underwent meticulous scrutiny, with each column examined to identify and address issues such as missing values, duplicates, and outliers.
2. Data Transformation: Categorical data within the churn column underwent transformation into numerical representations. This transformation facilitated the incorporation of these categorical variables into the analytical models, enhancing the depth and accuracy of our insights.
3. Exploratory Data Analysis (EDA): Extensive EDA was conducted. These analyses provided valuable insights into the distribution of features and the target variable, as well as uncovering potential correlations between different features within the dataset.
4. Feature Engineering: To augment the predictive power of the models, certain columns underwent feature engineering. This involved encoding categorical variables such as international_plan and voice_mail_plan into numerical representations, thereby enabling their inclusion in the analytical frameworks. Additionally, features were normalized and scaled to ensure uniformity and consistency across the dataset, leveraging techniques such as StandardScaler to achieve this objective.

### Modeling 
Three types of models: Logistic Regression, Random Forest and Decision Trees.

#### Logistic Regression

- Had an accuracy of 85.46%, F1-score of 26.67%, and AUC of 0.83.
#### Random Forest
- Attained an accuracy of 94.75%, F1-score of 80%, and AUC of 0.94.
- Hyperparameter tuning was executed leveraging GridSearchCV to optimize the Random Forest model.
#### Decision Trees:

- The model yielded an accuracy of 93.1%, and AUC of 0.85. 
#### Models Evaluation

ROC curves compared the performance of Decision Trees, Logistic Regression and Random Forest models, with Random Forest having a higher AUC.

#### Feature Importance
The following were the top predictors of churning: 
- Total day minutes
- Customer service calls
- Total evening minutes
![alt text](<feature importance.png>)
### Observations

- The Random Forest model outperforms both Logistic Regression and Decision Tree models in terms of AUC, with the highest value of 0.94.
- The Decision Tree model performs slightly better than Logistic Regression, with an AUC of 0.85 compared to 0.83.
- AUC is a measure of the classifier's ability to distinguish between classes, with higher values indicating better performance in separating the positive and negative instances.

In summary, the Random Forest model stands out as the top performer based on AUC, demonstrating its effectiveness in classifying the data. However, further analysis and validation are recommended to confirm the robustness of the findings and ensure generalizability to unseen data.

### Conclusions
The churn prediction analysis conducted for SyriaTel aimed to develop a classifier to identify customers likely to terminate their services. Through comprehensive data exploration, preparation, and modeling, several key findings emerged:

- Model Performance: Random Forest emerged as the most effective model for churn prediction, outperforming Logistic Regression and Decision Trees. It exhibited superior accuracy and predictive power, making it the preferred choice for SyriaTel's churn prediction system.
- Key Predictive Features: Total day minutes, customer service calls, and total evening minutes were identified as crucial indicators of churn. These insights provide valuable guidance for SyriaTel in devising proactive retention strategies targeted at high-risk customers.

### Recommendations

1. Enhance Call Quality: Invest in infrastructure and technology to improve call quality, ensuring a better customer experience.
2. Customer Service Improvement: Focus on enhancing customer service by reducing response times, increasing efficiency in issue resolution, and offering personalized support.
3. Proactive Retention Strategies: Implement proactive measures such as targeted promotions, loyalty rewards, and personalized communication to retain at-risk customers.
4. Regular Analysis: Continuously monitor customer behavior and churn patterns, regularly updating models and strategies to adapt to changing market dynamics.

### Next Steps

1. Increase Training Data Size: Expand the training dataset to reduce overfitting and improve model performance.
2. Targeted Recall Score: Aim to achieve the targeted recall score of 85% by refining the model and addressing overfitting issues.
3. Cost-Effective Customer Retention Strategies: Implement cost-effective strategies addressing key factors driving customer churn, such as personalized offers or discounts on day charges.

By implementing these recommendations and refining the modeling approach, SyriaTel can develop robust customer retention strategies to minimize churn and maximize customer satisfaction and revenue retention.