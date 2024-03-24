# Campus Recruitment Prediction With Machine Learning for MBA Students

This repository contains a machine learning project aimed at predicting campus placements for students using the Campus Recruitment dataset from Kaggle. The project involves exploratory data analysis (EDA), data preprocessing, and the implementation of a machine learning model to predict student placements in corporations.

## Dataset
The dataset used in this project can be found on Kaggle at the following link:
[Campus Recruitment Dataset](https://www.kaggle.com/datasets/benroshan/factors-affecting-campus-placement/data)

The dataset consists of various features that might influence the placement of students in jobs. The target variable is the "status" column, indicating whether a student is placed or not.

### Dataset Features
- sl_no: Serial Number
- gender: Gender (Male='M', Female='F')
- ssc_p: Secondary Education percentage (10th Grade)
- ssc_b: Board of Education (Central/ Others)
- hsc_p: Higher Secondary Education percentage (12th Grade)
- hsc_b: Board of Education (Central/ Others)
- hsc_s: Specialization in Higher Secondary Education
- degree_p: Degree Percentage
- degree_t: Under Graduation (Degree type) - Field of degree education
- workex: Work Experience
- etest_p: Employability test percentage (conducted by college)
- specialisation: Post Graduation (MBA) - Specialization
- mba_p: MBA percentage
- status: Status of placement (Placed/Not placed)
- salary: Salary offered by corporate to candidates

## Task
The task involves exploring the dataset, preprocessing the data, and building a machine learning model to predict student placements. The project follows these steps:

1. Exploratory Data Analysis (EDA)
2. Data Preprocessing
3. Model Development
4. Model Evaluation

## Exploratory Data Analysis (EDA)

The EDA phase involves exploring the dataset to understand its structure, distribution, and relationships between variables. Key steps include:
- Identifying categorical and numerical features
- Descriptive analytics for numerical features
- Visualizations to understand the distribution of features and their relationships with the target variable

## Data Preprocessing

Data preprocessing involves handling missing data, encoding categorical features, and scaling numerical features. Key steps include:
- Handling missing data by imputation
- Encoding categorical features using one-hot encoding
- Scaling numerical features using standardization
- Handling the imbalance nature of the dataset using SMOTE (Synthetic Minority Over-sampling Technique)

## Model Development: Support Vector Classifier (SVC)

The machine learning model chosen for this project is the Support Vector Classifier (SVC). The model is developed using the imbalanced-learn pipeline along with Stratified K-Folds cross-validation and GridSearchCV to avoid data leakage during the training process.

### Model Evaluation

The model is evaluated based on various metrics, including accuracy, confusion matrix, classification report, and ROC curve.

#### Classification Report

The classification report for the test set is as follows:

|           | Precision | Recall | F1-Score | Support |
|-----------|-----------|--------|----------|---------|
| Placed (0)   | 1.00      | 0.92   | 0.96     | 12      |
| Not Placed (1) | 0.97      | 1.00   | 0.98     | 31      |
| **Accuracy** | -       | -      | **0.98** | **43**  |
| **Macro Avg** | 0.98      | 0.96   | 0.97     | 43      |
| **Weighted Avg** | 0.98   | 0.98   | 0.98     | 43      |

The classification report provides precision, recall, F1-score, and support for each class (Placed and Not Placed), along with accuracy, macro-average, and weighted-average scores. The model achieves an overall accuracy of 98% on the test set, indicating high predictive performance.

## Conclusion

The Support Vector Classifier model demonstrates strong predictive performance in determining student placements based on the provided dataset. The project showcases the importance of exploratory data analysis, data preprocessing, and robust model evaluation techniques in machine learning tasks.
