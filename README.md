# Email Spam Classification Project

This project focuses on building a machine learning model to classify emails as either spam or not spam (ham). The dataset used contains email messages labeled with their respective categories.

## Dataset

The dataset used in this project is a collection of emails labeled as spam or ham. It consists of two main columns:

- **Category**: Indicates whether the email is spam or ham.
- **Message**: The content of the email.

### Dataset Details

- **Total Rows**: 5572
- **Columns**:
  - **Category**: Categorical (ham or spam)
  - **Message**: Text data

## Methodology

### Data Preprocessing

1. **Loading the Dataset**: The dataset is loaded using Pandas, a Python library for data manipulation and analysis.
2. **Data Cleaning**: Checked for any missing values, none were found.
3. **Feature Engineering**: Created a binary target variable (`Spam`) based on the `Category` column for model training.

### Model Building

#### Naive Bayes Classifier

- **Description**: Used the Multinomial Naive Bayes classifier due to its effectiveness with text data.
- **Pipeline**: Integrated the CountVectorizer and Multinomial Naive Bayes into a single pipeline for text classification.
- **Accuracy**: Achieved an accuracy of approximately 97.7% on the test dataset.

#### Other Models Explored

1. **Random Forest Classifier**
   - **Description**: Ensemble learning method that constructs multiple decision trees during training and outputs the class that is the mode of the classes (classification) or mean prediction (regression) of the individual trees.
   - **Accuracy**: Achieved 100% accuracy on the test dataset.

2. **Bagging Classifier**
   - **Description**: Implemented using the Gaussian Naive Bayes as the base estimator, which aggregates multiple models to improve accuracy.
   - **Accuracy**: Achieved 99.17% accuracy on the training dataset.

### Model Evaluation

- **Accuracy Scores**:
  - Multinomial Naive Bayes: 97.7%
  - Random Forest Classifier: 100%
  - Bagging Classifier: 99.17%

### Conclusion

This project successfully demonstrates the application of machine learning techniques for email spam classification. The models explored achieved high accuracy in distinguishing between spam and ham emails. Further improvements could involve tuning hyperparameters, exploring additional models, or utilizing more advanced natural language processing techniques.

---

