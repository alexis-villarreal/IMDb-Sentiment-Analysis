# IMDb Movie Review Sentiment Analysis

## Overview

This project uses Natural Language Processing (NLP) and machine learning to classify IMDb movie reviews as either positive or negative.

The goal was to compare multiple machine learning classification models and identify the model that performed best at predicting sentiment.

## Dataset

The project uses the IMDb Dataset of 50K Movie Reviews.

- 50,000 total movie reviews
- Binary sentiment classification: positive or negative
- A 10,000-review sample was used for modeling
- The sample initially contained 9,000 positive and 1,000 negative reviews
- Random undersampling was used to create a balanced dataset of 2,000 reviews

## Technologies

- Python
- Pandas
- NumPy
- Scikit-learn
- Seaborn
- Matplotlib
- TF-IDF
- GridSearchCV

## Machine Learning Models

Four classification models were trained and compared:

1. Support Vector Machine (SVM)
2. Logistic Regression
3. Decision Tree
4. Naive Bayes

## Results

| Model | Accuracy |
|---|---:|
| SVM | 84.09% |
| Logistic Regression | 83.03% |
| Decision Tree | 65.45% |
| Naive Bayes | 63.48% |

The Support Vector Machine achieved the highest accuracy at 84.09%.

### SVM Evaluation

- Positive F1 Score: 84.67%
- Negative F1 Score: 83.46%
- Overall Accuracy: 84.09%

## Model Tuning

GridSearchCV was used to test 10 combinations of SVM hyperparameters using 5-fold cross-validation.

The best parameters were:

- C = 1
- Kernel = linear

## Conclusion

The Support Vector Machine was the best-performing model among the four classifiers tested. It achieved 84.09% accuracy and demonstrated relatively balanced performance across positive and negative reviews.
