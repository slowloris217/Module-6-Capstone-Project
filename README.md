# Capstone Project
## SMS Spam Detection using Machine Learning
This project focuses on predicting whether an SMS message is spam or not using a dataset of various messages labeled as either spam or not spam. Detailed information about the dataset and the project can be found here: https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset/data

The project explores two distinct methods for preparing the data:

## Method 1: Text Preprocessing and Vectorization
In this method, we apply Natural Language Processing (NLP) techniques to preprocess the SMS messages by reducing words to their base or root form (stemming). We then use CountVectorizer to convert the processed text into numerical features that can be fed into the machine learning models.

## Method 2: Feature Engineering
In the second method, we focus on feature engineering by creating multiple variables that quantify various characteristics of each SMS message. These engineered features are then used as inputs for the models.

This dual approach allows us to explore different ways of preparing and utilizing the data, ultimately helping to identify the most effective method for detecting spam in SMS messages.

## Models Used:
- Logistic Regression: A simple yet powerful linear model that is often effective for binary classification tasks.
- K-Nearest Neighbors (KNN) Classifier: A non-parametric algorithm that classifies messages based on the majority class of their nearest neighbors.
- Random Forest Classifier: An ensemble method that uses multiple decision trees to improve accuracy and reduce overfitting.
- Support Vector Classifier (SVC): A robust model that seeks to find the optimal hyperplane that best separates the classes.

## Conclusion
  In conclusion, the final model chosen was the Random Forest model (rfc2) as it achieved the highest accuracy score of 0.9815 using the second approach, which focused on feature engineering. The model's effectiveness was further demonstrated when it accurately predicted a new input as spam, showcasing its ability to generalize well to unseen data. 

  Interestingly, while the KNN model performed the worst with the first method (scoring 0.9166, only slightly better than the null accuracy of 0.8659), it showed significant improvement with the second method, achieving an accuracy of 0.9797. This highlights how different models can perform better depending on the data preparation approach used, emphasizing the importance of tailoring data processing techniques to the specific strengths of each model.
