# EasyVisa-ML
"Advanced machine learning project featuring multiple ensemble methods and hyperparameter tuning using Randomized Search CV and Grid Search CV to optimize model performance.
# Easy-Visa Machine Learning Project

## Overview
Advanced machine learning project for visa approval prediction using ensemble methods and hyperparameter optimization to achieve high recall performance.

## Project Workflow

### 1. Data Understanding & Preprocessing
- **Data Exploration**: Analyzed dataframes, data types, and statistical summaries
- **Initial Assessment**: Understanding feature distributions and target variable characteristics

### 2. Exploratory Data Analysis (EDA)
- **Pair Plots**: Visualized relationships between numerical features
- **Heat Maps**: Examined correlation patterns and feature dependencies
- **Data Insights**: Identified key patterns and relationships in the dataset

### 3. Data Cleaning & Outlier Treatment
- **Outlier Detection**: Identified anomalous data points affecting model performance
- **Imputation Techniques**: Applied statistical methods to handle outliers and missing values
- **Data Quality**: Ensured clean, consistent dataset for modeling

### 4. Data Splitting Strategy
- **Train/Validation/Test Split**: Proper data partitioning to prevent data leakage
- **Test Set Protection**: Kept test set untouched throughout development process
- **Validation Framework**: Used validation set for model selection and tuning

### 5. Baseline Ensemble Modeling
- **Base Estimator**: Decision Tree as foundation for ensemble methods
- **Ensemble Techniques**: Tested multiple ensemble approaches ( ADA Boost, Gradient Boost, XGBoost, Bagging , RandomForest)
- **Metric Focus**: Prioritized **recall score** as primary evaluation metric
- Why Recall Matters for Visa Predictions
1. Cost of False Negatives is High
False Negative = Predicting "DENY" when visa should be "APPROVED"
This means qualified applicants get rejected
Real-world impact: Legitimate travelers/workers/students are unfairly denied
Business cost: Lost revenue, damaged reputation, legal issues

### 6. Class Imbalance Handling
- **SMOTE (Oversampling)**: Synthetic Minority Oversampling Technique for minority class augmentation
- **RUS (Undersampling)**: Random Under Sampling for majority class reduction
- **Balanced Dataset**: Improved class distribution for better model performance

### 7. Model Optimization & Selection
- **Re-evaluation**: Tested all ensemble methods on balanced dataset
- **Performance Comparison**: Selected model with highest recall on validation set
- **Model Selection**: Chose optimal ensemble approach based on validation metrics

### 8. Hyperparameter Tuning
- **RandomSearch CV**: Efficient hyperparameter space exploration
- **Grid Search CV**: Fine-tuned parameters for optimal performance
- **Cross-Validation**: Robust parameter selection with multiple validation folds

## Results
- **Final Test Recall**: **0.98** - Exceptional recall performance on unseen test data
- **Robust Method**: Comprehensive approach ensuring reliable, generalizable model
- **Production Ready**: High-performance model suitable for real-world visa prediction

## Key Features
- Comprehensive EDA with advanced visualizations
- Proper data leakage prevention
- Multiple ensemble method comparison
- Advanced sampling techniques (SMOTE & RUS)
- Systematic hyperparameter optimization
- Outstanding recall performance (98%)

## Technologies Used
- Python
- Pandas, NumPy for data manipulation
- Matplotlib, Seaborn for visualization
- Scikit-learn for machine learning
- Imbalanced-learn for sampling techniques
- Ensemble methods and hyperparameter tuning

---
*This project demonstrates end-to-end machine learning workflow with focus on achieving high recall for critical visa approval predictions.*
