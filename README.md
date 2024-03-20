# Capstone-Project

**Executive Summary**
In the dynamic world of e-commerce, ensuring timely delivery is a cornerstone for achieving customer satisfaction and fostering loyalty. The importance of predicting delivery times accurately cannot be overstated, as delays can lead to customer dissatisfaction, negative feedback, and a decline in repeat business. Conversely, precise delivery predictions can significantly improve operational efficiency, manage customer expectations more effectively, and potentially reduce costs associated with expedited shipping or compensations for delays. This analysis aims to provide non-AI/ML personnel with insights into how different aspects of the order process impact delivery times, enabling informed decision-making to enhance the customer experience.

The core research question addresses the feasibility of accurately predicting on-time delivery of online orders using customer and order data. Utilizing a dataset from Kaggle comprising approximately 11,000 observations across 12 variables, this analysis employed various machine learning classification methods, including logistic regression, decision trees, and random forests, complemented by exploratory data analysis (EDA) and feature engineering to enhance model performance.

The EDA phase was pivotal in understanding the dataset’s structure, evaluating the distribution of variables, and identifying preprocessing needs. Following this, data preprocessing involved encoding categorical variables, standardizing numerical features, and partitioning the dataset for model training. Feature engineering further refined the dataset by introducing a new variable to assess the impact of discount size relative to product cost on delivery timeliness.

Among the initial 3 models tested (Logisitic Regression, Decision Tree Classifier, Random Forest), the Random Forest classifier emerged as the most effective, showcasing superior accuracy (0.67), precision (0.79), recall (0.61), and AUC-ROC score (0.68). Subsequent exploration of more advanced models like Gradient Boosting Machine (GBM) and Extreme Gradient Boosting (XGBoost) revealed GBM as the top performer in accuracy (0.69), while XGBoost did not meet expectations.

This analysis illuminates several avenues for future research and optimization. The next steps involve refining feature engineering techniques, exploring more advanced modeling methods, and further tuning model parameters. These strategies aim to enhance the predictive accuracy of delivery times, which, in turn, can significantly improve customer satisfaction and operational efficiency in e-commerce logistics. 

**Rationale**
Understanding and predicting on-time delivery is crucial for maintaining customer satisfaction and loyalty in e-commerce. Late deliveries can lead to customer dissatisfaction, negative reviews, and a loss of repeat business. Conversely, accurate predictions of delivery times can aid in managing customer expectations, improving operational efficiency, and potentially reducing costs associated with expedited shipping or compensations for late deliveries. For non-AI/ML personnel, this analysis will offer insights into which aspects of the order process most significantly impact delivery times, enabling them to make informed decisions to enhance customer experience.

**Research Question:**
Can I accurately predict whether an online order will be delivered on time or not, using customer and order data?

**Data Source:**
The analysis utilized a dataset from Kaggle. This dataset contains ~11,000 observations of 12 variables, including customer ID, warehouse block, mode of shipment, customer care calls, customer rating, cost of the product, prior purchases, product importance, gender, discount offered, weight in grams, and the target variable indicating timely delivery.

**Methodology:**
The analysis employed various machine learning classification techniques, including logistic regression, decision trees, and random forests, to predict the on-time delivery of orders. These methods were complemented by exploratory data analysis to understand data distributions and relationships, and feature engineering to enhance model performance. Model evaluation was based on metrics including accuracy, precision, recall, and the AUC-ROC curve.

Upon loading the dataset, I embarked on a comprehensive exploratory data analysis (EDA). This step was important in understanding the dataset's structure, assessing the distribution of both numerical and categorical variables, and identifying any immediate preprocessing needs. No missing values were detected, and the distributions suggested a well-balanced dataset regarding the target variable.

Data preprocessing involved several steps to ensure the dataset was primed for modeling. I encoded categorical variables to transform them into a machine-readable format, standardized numerical features to mitigate scale discrepancies, and partitioned the dataset into training and testing sets.

In the pursuit of enhancing model performance, I engaged in feature engineering, creating a new variable that encapsulated the ratio of discount offered to the cost of the product. This feature aimed to uncover any potential influence of relative discount size on delivery timeliness. The dataset was then scrutinized for feature relevance, setting the stage for model training.

**Results:**
I trained several models, including Logistic Regression, Decision Tree, and Random Forest, to predict on-time delivery. The Random Forest model was identified as the most promising, based on metrics such as accuracy, precision, recall, and AUC-ROC score. This model underwent further optimization through hyperparameter tuning, enhancing its predictive capability. Some more advanced models, Gradient Boosting Machine (GBM) and Extreme Gradient Boosting (XGBoost), were also explored.

For the intial 3 models, the Random Forest outperformed others, showcasing the highest accuracy and demonstrating its robustness in handling the dataset's complexities. This result underscores the model's effectiveness in predicting on-time delivery, a critical insight for e-commerce logistics. For the advanced models, GBM showed the best accuracy score overall, while XGBoost did not perform well.

**Next Steps**
This analysis revealed areas for improvement, including refining feature engineering, exploring advanced modeling techniques, and further optimizing model parameters. These opportunities suggest a path forward for enhancing predictive accuracy and, by extension, customer satisfaction in e-commerce operations.


