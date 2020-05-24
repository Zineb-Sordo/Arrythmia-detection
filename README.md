# Arrythmia-detection

This project is a binary classification problem aiming at predicting Arrythmia based on the UCI ML Repository arrhythmia data set: 
http://localhost:8888/edit/Desktop/Data%20science%20shit/Arrythmia%20prediction%20project%20/arrhythmia.data
http://localhost:8888/edit/Desktop/Data%20science%20shit/Arrythmia%20prediction%20project%20/arrhythmia.names

Pipeline: 
  I - Import data and first interpretation
    - Null values 
    - Columns with identical values 
    - Data distribution 
    - PCA
  II - Binary classification 
    - Create 2 classes to get down to a binary classification problem 
    - Oversampling 
    - ML models (Naive Bayes, Logistic Regression, KNN, SVM, Decision Tree, XGBoost, Random Forest)
    - Random Forest:
      - Parameter tuning with Gridsearch
      - Feature selection with RFECV
      - Feature selection using mutual information
      - Testing the model 
    - XGBoost: same steps than for Random Forest
    - SHAP visualization 

I achieved 84% testing accuracy using a fine-tuned Random Forest Classifier and 82% accuracy using a fine-tuned XGBoost Classifier. 

The difficulty of this project was to avoid overfitting and deal with the smallness of the test set (91 samples for a 20% test split). 
