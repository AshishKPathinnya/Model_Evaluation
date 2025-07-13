Wine Dataset Classification Project
Overview

This project focuses on classifying wine types based on their chemical analysis using various machine learning models. The goal is to identify the best-performing model for this classification task by training, tuning, and evaluating several popular algorithms.
Project Steps

    Data Loading: The Wine dataset, a classic dataset for classification and pattern recognition problems, is loaded from the scikit-learn library.
    Data Splitting: The dataset is split into training and testing sets to prepare for model training and evaluation. An 80/20 split is used for training and testing, respectively.
    Model Definition: Multiple classification models are defined for evaluation, including:
        Logistic Regression
        Support Vector Classifier (SVC)
        Decision Tree Classifier
        K Neighbors Classifier
    Hyperparameter Tuning: To optimize the performance of each model, hyperparameter tuning is performed using:
        GridSearchCV for Logistic Regression, SVC, and K Neighbors Classifier.
        RandomizedSearchCV for Decision Tree Classifier.
        Model Training and Evaluation: Each model is trained using the training data and the best hyperparameters found during tuning. Their performance is then evaluated on the unseen test set using the following metrics:
        Accuracy
        Precision
        Recall
        F1-score
    Results Analysis: The evaluation results are analyzed to compare the performance of the different models and identify the best one based on the chosen metrics, particularly the F1-score.

Results

The models were evaluated based on their performance on the test set after hyperparameter tuning. The evaluation metrics for each model are summarized below:


Model 	                     Accuracy Precision   Recall   	F1-score
LogisticRegression 	         0.9722 	0.9741      0.9722  	0.9722
SVC 	                       1.0000 	1.0000      1.0000 	  1.0000
DecisionTreeClassifier 	     0.9444 	0.9514 	    0.9444 	  0.9449
KNeighborsClassifier 	       0.7500 	0.7599 	    0.7500  	0.7524

Based on the F1-score and other evaluation metrics, the Support Vector Classifier (SVC) model achieved the highest performance, with perfect scores across all metrics on the test set.
Conclusion

The project successfully trained and evaluated multiple machine learning models for classifying the Wine dataset. The hyperparameter tuning process helped optimize the models' performance. The SVC model demonstrated superior performance on the test set, making it the best-performing model for this classification task among the evaluated algorithms.
