# MachineLearning-CreditCardChurners

### Project Summary
The Credit Card Churners project analyzes customer attrition for a financial institution, aiming to identify factors that influence customer churn and develop predictive models to prevent attrition. By understanding customer demographics, spending behavior, and engagement with the institution, the project informs data-driven strategies to improve customer retention.

### Key Aspects of the Project
#### Data Exploration: 
Analyzed customer demographic and behavioral data to understand attrition trends and patterns.
#### EDA Insights: 
Investigated distributions of features such as transaction amounts, education levels, and income categories. Key questions explored included attrition variation across demographics and the significance of feature correlations.
#### Feature Engineering: 
Focused on selecting the most relevant features for the model, based on correlation and importance analyses.
#### Model Selection: 
Employed multiple classification models (AdaBoost, Gradient Boost, XGBoost) with undersampling and oversampling techniques, selecting models that balanced recall and generalization.

### Statistical Analysis
#### Demographic Analysis: 
Examined age, gender, and marital status distributions. Most customers were middle-aged, with a slight gender imbalance (more female customers).
#### Customer Behavior: 
Attrition correlated with low credit limits, minimal transactions, and inactive months. Monthly inactivity and communication frequency showed a potential link to attrition rates.
#### Correlation: 
Features such as credit limit and available credit were highly correlated, as were transaction amounts with total amount and count changes, leading to a selection of non-redundant features.

### Data Processing and Model Building
#### Data Preprocessing: 
Cleaned the dataset by addressing missing values, removing irrelevant columns (e.g., Client Number), and encoding categorical variables.
#### Feature Engineering: 
Identified five key features with the highest predictive power: Total Transaction Count, Total Transaction Amount, Total Revolving Balance, Total Count Change (Q4 to Q1), and Total Amount Change (Q4 to Q1).
#### Model Training: 
Implemented and tuned AdaBoost, Gradient Boosting, and XGBoost classifiers, with recall as the primary evaluation metric. Both undersampling and oversampling were used to address class imbalance.
#### Model Evaluation: 
Focused on recall to minimize false negatives. The XGBoost model, especially with undersampled and oversampled data, demonstrated high recall but some risk of overfitting, while undersampled AdaBoost and Gradient Boost models achieved balanced performance.

### Takeaways from the Project
#### Attrition Insights: 
Customers with fewer bank products, lower credit limits, and less transaction activity were more likely to churn. Attrition was also higher among older age groups and those with fewer interactions with the bank.
#### Model Insights: 
Models trained with undersampled data often performed better in recall, highlighting the importance of balancing classes for effective attrition prediction.
#### Business Recommendations: 
To reduce attrition, the institution could focus on engagement strategies for at-risk customers, especially those with low transaction volumes or infrequent use of bank products.


