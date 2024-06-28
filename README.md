Income Prediction Using UCI Adult Dataset

Introduction:
This repository contains the code and notebook for a project focused on predicting whether an individual's income exceeds $50K/year based on census data from the UCI Adult dataset. 
The project involves data preprocessing, exploratory data analysis, and training a Support Vector Machine (SVM) model.

Dataset:
The dataset used for this project is the Adult training dataset available at the UCI Machine Learning Repository. 
The dataset includes various demographic attributes such as age, education, occupation, and income.

Implementation Details:

1. Data Import: The dataset is imported directly from the UCI Machine Learning Repository without saving it locally.
2. Data Exploration: Performed initial data exploration using .head(), .info(), .describe(), and .shape to understand the structure of the dataset.
3. Data Visualization: Plotted histograms of the data to visualize distributions.
4. Missing Values: Identified and replaced missing values represented as '?' with nan and updated the dataset.
5. Preprocessing Pipeline: Created a preprocessing pipeline to-
     - Fill missing numerical values with the mean.
     - Scale numerical columns using StandardScaler.
     - Fill missing categorical values with the most frequent value.
     - Encode categorical columns using OneHotEncoder.
     - Target Value Cleaning
     - Reviewed and cleaned the target values to remove periods from the income categories for consistency.

6. Train-Test Split: Split the dataset into training and testing sets with an 80-20 split.
7. Model Training: Trained an SVM model using a polynomial kernel with specific hyperparameters (gamma=1 and C=0.1).
8. Model Evaluation: Evaluated the model using classification_report and confusion matrix.
9. Hyperparameter Tuning: Utilized GridSearchCV to find the best hyperparameters and performed additional train-validation-test splits.

Results:
The results of the model training and evaluation, including accuracy, precision, recall, F1-score, and confusion matrix, are provided in the notebook.

Acknowledgments:
The dataset used is provided by the UCI Machine Learning Repository. Special thanks to Dr. Ruba Alomari for guidance and support.
