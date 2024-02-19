# Capstone-Project

**Problem Statment**

**Research Question:**
Can I accurately predict whether an online order will be delivered on time or not, using customer and order data?

**Data Source:**
The analysis will utilize a dataset from Kaggle. This dataset contains 10,999 observations of 12 variables, including customer ID, warehouse block, mode of shipment, customer care calls, customer rating, cost of the product, prior purchases, product importance, gender, discount offered, weight in grams, and the target variable indicating timely delivery.

**Techniques for Analysis:**
The analysis will employ various machine learning classification techniques, such as logistic regression, decision trees, and random forests, to predict the on-time delivery of orders. These methods will be complemented by exploratory data analysis to understand data distributions and relationships, and feature engineering to enhance model performance. Model evaluation will be based on metrics like accuracy, precision, recall, and the AUC-ROC curve.

**Expected Results:**
I anticipate identifying key factors that influence the timely delivery of online orders. The model is expected to provide a reliable prediction of whether an order will be delivered on time, based on the input variables.

**Importance of the Question:**
Understanding and predicting on-time delivery is crucial for maintaining customer satisfaction and loyalty in e-commerce. Late deliveries can lead to customer dissatisfaction, negative reviews, and a loss of repeat business. Conversely, accurate predictions of delivery times can aid in managing customer expectations, improving operational efficiency, and potentially reducing costs associated with expedited shipping or compensations for late deliveries. For non-AI/ML personnel, this analysis will offer insights into which aspects of the order process most significantly impact delivery times, enabling them to make informed decisions to enhance customer experience.




**Analysis**
In this project, my primary goal was to address a critical challenge faced by e-commerce businesses: the ability to predict whether an online order will be delivered on time. This issue is not merely operational; it touches the core of customer satisfaction and loyalty, areas where the margin for error is slim. Late deliveries can significantly impact customer trust and brand reputation, making accurate predictions a valuable asset for any e-commerce entity.

**Data Exploration and Preparation**
The analysis was underpinned by a dataset sourced from Kaggle, encompassing approximately 11,000 observations across 12 variables. These variables included both customer and order details such as warehouse block, mode of shipment, customer care calls, cost of the product, and the crucial target variable indicating timely delivery.

Upon loading the dataset, I embarked on a comprehensive exploratory data analysis (EDA). This step was instrumental in understanding the dataset's structure, assessing the distribution of both numerical and categorical variables, and identifying any immediate preprocessing needs. No missing values were detected, and the distributions suggested a well-balanced dataset regarding the target variable.

**Data Preprocessing**
Data preprocessing involved several steps to ensure the dataset was primed for modeling. I encoded categorical variables to transform them into a machine-readable format, standardized numerical features to mitigate scale discrepancies, and partitioned the dataset into training and testing sets. This preparation was vital for the subsequent modeling phase.

**Feature Engineering and Selection**
In the pursuit of enhancing model performance, I engaged in feature engineering, creating a new variable that encapsulated the ratio of discount offered to the cost of the product. This feature aimed to uncover any potential influence of relative discount size on delivery timeliness. The dataset was then scrutinized for feature relevance, setting the stage for model training.

**Model Development and Optimization**
I trained several models, including Logistic Regression, Decision Tree, and Random Forest, to predict on-time delivery. The Random Forest model was identified as the most promising, based on metrics such as accuracy, precision, recall, and AUC-ROC score. This model underwent further optimization through hyperparameter tuning, enhancing its predictive capability.

Some more advanced models, Gradient Boosting Machine (GBM) and Extreme Gradient Boosting (XGBoost), were also explored.

**Results and Conclusion**
For the intial 3 models, the Random Forest outperformed others, showcasing the highest accuracy and demonstrating its robustness in handling the dataset's complexities. This result underscores the model's effectiveness in predicting on-time delivery, a critical insight for e-commerce logistics. For the advanced models, GBM showed the best accuracy score overall, while XGBoost did not perform well.

This initial analysis revealed areas for improvement, including refining feature engineering, exploring advanced modeling techniques, and further optimizing model parameters. These opportunities suggest a path forward for enhancing predictive accuracy and, by extension, customer satisfaction in e-commerce operations.

In conclusion, this project is intended to help in identifying a reliable model for predicting on-time delivery but also highlighting the multifaceted nature of logistic challenges in e-commerce. The insights derived from this analysis are poised to inform strategic decisions, streamline operations, and ultimately, fortify customer trust and satisfaction in an increasingly competitive landscape.
