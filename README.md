# PREDICTING CUSTOMER CHURN IN THE TELECOMMUNICATION INDUSTRY

## NON-TECHNICAL EXPLANATION OF YOUR PROJECT
This project uses machine learning algorithms to predict customer churn behavior in the telecommunications industry. By analyzing anonymized customer data, it will identify patterns and factors that influence customer churn and develop a model that can predict which customers are likely to churn. This model has important implications for the telecommunications industry by providing valuable insights into customer behavior and enabling companies to develop more effective retention strategies. We also prioritize data privacy and ethical considerations by using anonymized customer data and ensuring that the model is not used for unethical or discriminatory purposes. This project demonstrates the potential of machine learning algorithms to inform decision-making in various industries and highlights the importance of responsible and ethical use of data.

## DATA
"Telco Customer Churn" is the dataset that has been used which is publicly available on Kaggle. The dataset contains information on customer demographics, services used, account information, and whether or not the customer has churned. Here is the link to the dataset (https://www.kaggle.com/datasets/blastchar/telco-customer-churn).

## MODEL 
This project has used an ensemble model that combines three classifiers: AdaBoost, Logistic Regression, and Neural Network. These classifiers are effective at predicting customer churn based on different factors and patterns. The ensemble model was chosen because it provides more robust and decent prediction results compared to a single classifier.

## HYPERPARAMETER OPTIMIZATION
This project optimized the hyperparameters of each classifier using Bayesian Optimization before the Voting classifier was applied. This method allowed us to efficiently search for the best combination of hyperparameters that maximize the performance of the classifier. We chose to optimize the hyperparameters of each classifier separately to ensure that each classifier is optimized for its own specific features and patterns.

## RESULTS
The final model has achieved a decent accuracy of 80.05% using a Voting Classifier that combines the three classifiers. The precision and recall were 79.04% and 80.05%, respectively, with an F1 score of 79.25%. These results suggest that our model is reasonably effective at predicting customer churn behavior. However, our model has several limitations related to the dataset such as imbalanced data and limited external factors. These limitations should be taken into consideration when applying the model to new datasets or industries.
