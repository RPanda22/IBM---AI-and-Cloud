# Fake Instagram Account Detection

## Table of Contents
1. [Introduction](#introduction)
2. [Problem Statement](#problem-statement)
3. [Proposed Solution](#proposed-solution)
4. [System Development Approach](#system-development-approach)
5. [Algorithms and Deployment](#algorithms-and-deployment)
6. [Results](#results)
7. [Conclusion](#conclusion)

## Introduction
With the rapid growth of social media platforms, the prevalence of fake accounts has become a significant issue. These accounts can be used for spamming, spreading misinformation, and fraudulent activities. This project aims to develop a machine learning-based solution to identify and flag fake Instagram accounts based on various account attributes.

## Problem Statement
Fake accounts on Instagram can disrupt the user experience and pose security risks. Identifying these accounts manually is impractical due to the vast number of users. Therefore, there is a need for an automated solution that can accurately detect fake accounts using machine learning techniques.

## Proposed Solution
The solution involves developing a machine learning classifier to detect fake Instagram accounts. By analyzing various account features, the classifier can distinguish between genuine and fake accounts. The project utilizes several machine learning algorithms, evaluates their performance, and selects the best model for deployment.

## System Development Approach
The development approach includes the following steps:
1. **Data Collection**: The dataset `instaFake.csv` includes features such as `edge_followed_by`, `edge_follow`, `username_length`, `username_has_number`, `full_name_has_number`, `full_name_length`, `is_private`, `is_joined_recently`, `has_channel`, `is_business_account`, `has_guides`, `has_external_url`, and `is_fake`.
2. **Data Preprocessing**: Handling missing values, feature scaling, and splitting the data into training and validation sets.
3. **Model Training**: Training multiple machine learning models including XGBoost, AdaBoost, CatBoost, and LightGBM.
4. **Model Evaluation**: Evaluating the models using metrics such as accuracy, precision, recall, F1-score, and confusion matrix.
5. **Model Selection**: Selecting the best-performing model for deployment.

## Algorithms and Deployment
The project uses the following machine learning algorithms:
- **XGBoost**: An implementation of gradient-boosted decision trees designed for speed and performance.
- **AdaBoost**: A boosting algorithm that combines multiple weak classifiers to form a strong classifier.
- **CatBoost**: A gradient-boosting algorithm that handles categorical features well.
- **LightGBM**: A gradient-boosting framework that uses tree-based learning algorithms.

### Model Evaluation
Each model is evaluated based on:
- **Accuracy**: Proportion of correctly classified instances.
- **Precision**: Proportion of true positive instances among the predicted positives.
- **Recall**: Proportion of true positive instances among the actual positives.
- **F1-Score**: Harmonic mean of precision and recall.
- **Confusion Matrix**: Visualization of the true positives, true negatives, false positives, and false negatives.

### Best Model Deployment
The XGBoost model achieved the highest accuracy of 0.9618 and was selected as the best model. It was further tuned and deployed for real-time fake account detection. The model's performance was visualized using various plots and graphs to illustrate its effectiveness.

## Results
- **XGBoost Accuracy**: 0.9618
- **Evaluation Metrics**: The classification report and confusion matrix demonstrated the model's strong performance.
- **Feature Importance**: Key features influencing the model's predictions were identified.
- **Visualization**: Plots of the actual vs. predicted labels for the top 20 samples.

## Conclusion
The project successfully developed a machine learning solution to detect fake Instagram accounts. The XGBoost model demonstrated high accuracy and robustness, making it suitable for real-time application. The results highlight the model's ability to generalize well on unseen data, providing an efficient solution for enhancing the security and integrity of Instagram profiles.

---

**Project developed by Roshan Panda during an AI and Cloud Internship at IBM.**

Feel free to explore the code, contribute, or raise issues if you encounter any problems. Thank you for your interest in this project!
