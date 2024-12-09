# Spam Classification Using Naive Bayes with Parameter Optimization
## Overview
This project focuses on classifying spam messages using the Naive Bayes algorithm. By comparing different text vectorization techniques (`CountVectorizer` and `TfidfVectorizer`) and tuning hyperparameters, we optimize the model for better performance.
## Features
- Baseline comparison of `CountVectorizer` and `TfidfVectorizer`.
- Hyperparameter tuning for Naive Bayes using `GridSearchCV`.
- Evaluation metrics: Classification report, confusion matrix, ROC-AUC curve.
## Dataset
The dataset used is a publicly available spam dataset:
- Source:(https://www.kaggle.com/uciml/sms-spam-collection-dataset)
- Size: 5,572 messages (ham and spam)
- ## Methodology
1. Data preprocessing and splitting into training and test sets.
2. Baseline models with default Naive Bayes settings.
3. Parameter tuning (`alpha`, `ngram_range`, `max_df`) using `GridSearchCV`.
4. Model evaluation with performance metrics.
- ## Results
Model Performance:

Accuracy: 98%
Precision (Class 0): 0.98, Recall (Class 0): 1.00, F1-Score (Class 0): 0.99
Precision (Class 1): 0.98, Recall (Class 1): 0.88, F1-Score (Class 1): 0.93
Overall Accuracy: 98%

Macro Average:

Precision: 0.98
Recall: 0.94
F1-Score: 0.96
Weighted Average:

Precision: 0.98
Recall: 0.98
F1-Score: 0.98

Install dependencies:
pip install -r requirements.txt

Run the Python script:
python spam_classifier.py

- ## File Structure
- .
├── data/
│   └── spam.csv                
├── spam_classifier.py        
├── report.pdf                 
├── requirements.txt           
└── README.md                   
