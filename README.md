# Wine Dataset Classification Project

## Overview

This project focuses on classifying wine types based on their chemical analysis using various machine learning models. The goal is to identify the best-performing model for this classification task by training, tuning, and evaluating several popular algorithms.

## Project Steps

1. **Data Loading**  
   The Wine dataset, a classic dataset for classification and pattern recognition, is loaded from the scikit-learn library.

2. **Data Splitting**  
   The dataset is split into training and testing sets using an 80/20 ratio for model training and evaluation.

3. **Model Definition**  
   Multiple classification models are defined for evaluation, including:
   - Logistic Regression  
   - Support Vector Classifier (SVC)  
   - Decision Tree Classifier  
   - K Neighbors Classifier  

4. **Hyperparameter Tuning**  
   To optimize each model's performance:
   - `GridSearchCV` is used for Logistic Regression, SVC, and K Neighbors Classifier.  
   - `RandomizedSearchCV` is used for the Decision Tree Classifier.  

5. **Model Training and Evaluation**  
   Each model is trained on the training data using the best hyperparameters found. The models are evaluated on the test set using:
   - Accuracy  
   - Precision  
   - Recall  
   - F1-score  

6. **Results Analysis**  
   The models' evaluation metrics are analyzed to compare their performance and identify the best model, particularly based on F1-score.

## Results

| Model                   | Accuracy | Precision | Recall  | F1-score |
|------------------------|----------|-----------|---------|----------|
| Logistic Regression     | 0.9722   | 0.9741    | 0.9722  | 0.9722   |
| SVC                     | 1.0000   | 1.0000    | 1.0000  | 1.0000   |
| Decision Tree Classifier| 0.9444   | 0.9514    | 0.9444  | 0.9449   |
| K Neighbors Classifier  | 0.7500   | 0.7599    | 0.7500  | 0.7524   |

Based on the F1-score and other evaluation metrics, the **Support Vector Classifier (SVC)** achieved the highest performance with perfect scores across all metrics.

## Conclusion

This project successfully implemented and evaluated multiple machine learning models for classifying wines using the Wine dataset. Hyperparameter tuning significantly improved model performance. The SVC model outperformed all others, making it the most effective choice for this classification task.
