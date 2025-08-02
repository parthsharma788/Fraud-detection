# Fraud-detection

## Description:

This project is a fraud detection pipeline designed to identify fraudulent activities using machine learning. It utilizes the XGBoost model, an optimized gradient boosting algorithm, which is particularly effective for tabular and imbalanced datasets like those commonly found in fraud detection.

To address the challenge of imbalanced data where fraud cases are rare, the pipeline incorporates the Synthetic Minority Over-sampling Technique (SMOTE) to create synthetic data points for the minority class. The pipeline also includes a feature engineering step with data scaling and numeric encodings.

The model's performance is optimized through cross-validated grid search for hyperparameter tuning, with the Precision-Recall Area Under the Curve (PR-AUC) as the primary evaluation metric, which is a more suitable metric for imbalanced classification problems than accuracy.

## Key Features:

XGBoost Model: Uses a powerful and efficient tree ensemble method.

SMOTE: Handles imbalanced data by oversampling the minority class.

Hyperparameter Tuning: Fine-tunes the model for optimal performance using cross-validated grid search.

PR-AUC Scoring: Evaluates model performance using a metric appropriate for imbalanced datasets.

Repository Contents:

FraudCSV.xlsx: The dataset used for training and evaluation.

feature_importance.csv: A file detailing the importance of each feature in the model.

confusion_matrix.png: A visual representation of the model's classification performance.

roc_curve.png: A graph showing the model's Receiver Operating Characteristic curve.

fraud_detection_pipeline.ipynb: The Jupyter Notebook containing the complete code for the project.
