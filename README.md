## Students Adaptability Prediction

### Project Overview

This project aims to predict the **adaptability level of students in online education** based on a variety of demographic, socioeconomic, and technology-related factors. By analyzing features such as gender, age, education level, financial condition, internet type, and device usage, the goal is to develop a machine learning model that can classify students into different adaptability levels (High, Moderate, or Low). This can help educational institutions and policymakers provide better support for online learners.

-----

### Technical Highlights

  * **Dataset**: [Kaggle - Students Adaptability Level in Online Education](https://www.kaggle.com/datasets/mdmahmudulhasansuzan/students-adaptability-level-in-online-education)
  * **Size**: 1205 entries, 14 columns.
  * **Key Features**:
      * All features are categorical, including `Gender`, `Age`, `Education Level`, `Institution Type`, `Financial Condition`, `Internet Type`, and `Device`.
  * **Approach**:
      * **Data Cleaning**: The dataset was clean with no missing values or duplicates.
      * **Exploratory Data Analysis**: Count plots were used to visualize the distribution of all categorical features.
      * **Label Encoding**: Applied to all columns to convert categorical data into numerical format for model training.
      * **Multi-class Classification**: The target variable `Adaptivity Level` has three classes: 'Low', 'Moderate', and 'High'. The dataset is imbalanced.
      * **Models Used**:
          * Logistic Regression, Ridge Classifier, SVC, Random Forest, XGBoost, AdaBoost, Gradient Boosting, Bagging, Decision Tree.
  * **Best Accuracy**:
      * 90.9% with Random Forest and Decision Tree Classifiers.
      * 90.5% with XGBoost and Bagging Classifiers.
      * 83.4% with Gradient Boosting Classifier.

-----

### Purpose and Applications

  * **Predict student adaptability** in online learning environments.
  * Help educational institutions identify students who may struggle and require additional support.
  * Inform the development of targeted interventions and resources to improve student engagement and success.
  * Provide insights for educational policy and online course design.

-----

### Installation

Clone the repository:

```bash
git clone https://github.com/BhaveshBhakta/Students-Adaptability-Prediction-Using-ML.git
cd Students-Adaptability-Prediction-Using-ML
```

Install the necessary libraries:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn xgboost
```

-----

### Collaboration

We welcome contributions to improve the project. You can help by:

  * Performing comprehensive hyperparameter tuning and cross-validation for all models to achieve optimal performance.
  * Investigating the impact of different encoding methods for categorical features (e.g., One-Hot Encoding vs. Label Encoding).
  * Exploring alternative methods for handling the class imbalance in the target variable, although the provided results are already very high.
  * Adding explainability (e.g., SHAP or LIME) to understand which student characteristics are the most significant predictors of their adaptability level.
