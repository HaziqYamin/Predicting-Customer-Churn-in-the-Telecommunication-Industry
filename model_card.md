# Model Card

## Model Description

**Input:** The inputs of this dataset would consist of the various features and variables included in the dataset. These features might include customer demographic information, customer account information, and service utilization data.

**Output:** The output of this dataset would be a binary classification label indicating whether or not the customer is likely to churn. Additionally, the model may output information on the relative importance of different features in predicting churn which could be used to inform business decisions and strategies.

**Model Architecture:** The model architecture consists of an ensemble of three classifiers: the AdaBoost Classifier, the Logistic Regression classifier, and the Neural Network classifier, and each is utilized to predict customer churn. In a simple explanation, the AdaBoost Classifier is an ensemble learning method that combines multiple weak classifiers to form a strong classifier, while Logistic Regression is a linear classification algorithm that models the probability of the target class as a function of the input features. Additionally, the Neural Network is a machine learning model that utilizes layers of interconnected nodes to capture complex nonlinear relationships in the data. Bayesian Optimization was applied to each classifier to optimize the hyperparameters and achieve better performance. The final predictions are produced by a Voting Classifier that aggregates the outputs of the individual models using a majority vote, reducing the risk of overfitting and enhancing the overall performance of the model.

## Model Performance/ Model Evaluation

The performance of the model was evaluated on the "Telco Customer Churn" dataset using several evaluation metrics including accuracy, precision, recall, and F1 score. The model achieved an accuracy of 80.05% which is the highest achieved by the Voting Classifier. The precision of the model was found to be 79.04%, and the recall was 80.05%, resulting in an F1 score of 79.25%. These metrics suggest that the model is effective in predicting customer churn, and it could aid in developing targeted retention strategies. Overall, the model shows promise in identifying customers who are likely to churn and has the potential to assist in reducing the churn rate and improving customer retention in the telecommunications industry.

## Limitations

The model has several limitations related to the dataset used. Firstly, the dataset is imbalanced which may result in biased predictions toward non-churn customers and false negatives. Secondly, the dataset only contains customer data from a single telecommunications company and may not be representative of customer churn behavior in other companies. Also, the model's performance may be impacted by the specific hyperparameters chosen during training, and these hyperparameters may not be optimal for other datasets. The model may also suffer from overfitting and may not generalize well to new data. Furthermore, the model's predictions may not consider the specific business context of the telecommunications company, and the strategies that work for one company may not be effective for others. Finally, the dataset does not include external factors that may impact customer churn such as economic or regulatory changes. These limitations highlight the need for caution when applying the model to new datasets or industries and the importance of considering external factors that may impact customer churn.

## Trade-offs 

The model has several trade-offs that should be considered when applying it to new datasets. Firstly, the model may have performance issues when the dataset contains missing or incomplete data which can lead to inaccurate or biased predictions. Secondly, the model may exhibit reduced accuracy, precision, and recall when applied to datasets with different distributions than this dataset. Moreover, churn behavior may be influenced by different factors in different industries that lead to performance issues when applying the model to datasets from different industries. Lastly, the model may require significant computational resources to train, particularly when the dataset is large or when the hyperparameter tuning process is extensive. These trade-offs should be taken into consideration when applying the model to new datasets or industries, and any potential performance issues should be addressed accordingly to ensure accurate and reliable predictions.