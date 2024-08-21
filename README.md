# Logistic Regression on Diabetes Dataset with StandardScaler

This project demonstrates the implementation of a Logistic Regression model using the Diabetes dataset. The dataset is used to predict whether a person has diabetes based on various health-related features. The project also explores the impact of feature scaling using `StandardScaler`.

## Project Overview

The objective is to classify individuals as diabetic or non-diabetic based on a set of input features. The dataset used in this project includes features such as Pregnancies, Glucose levels, Blood Pressure, Skin Thickness, Insulin levels, BMI, Diabetes Pedigree Function, Age, and a binary outcome (`Class`).

## Files

- **`diabetes.csv`**: The dataset file containing health-related features and the target class.
- **`Logistic_Regression_with_StandardScaler_on_CSV_File.ipynb`**: The Python script implementing the Logistic Regression model with and without feature scaling.
- **`README.md`**: This file, providing an overview of the project.

## Implementation Details

1. **Loading the Data**: The dataset is loaded using `pandas`, and the initial exploration includes checking the dataset's shape, structure, and a few samples.

2. **Data Preprocessing**:
   - The features (`X`) are separated from the target variable (`y`).
   - Feature scaling is performed using `StandardScaler` to normalize the input features.

3. **Model Training**:
   - The dataset is split into training and testing sets.
   - A Logistic Regression model is trained on both the original and scaled datasets.

4. **Model Evaluation**:
   - Predictions are made on the test set.
   - The performance of the model is evaluated using accuracy, confusion matrix, and classification report.
   - The classification report includes precision, recall, f1-score, and support for each class.

## Results

Both the models, with and without scaling, produced similar classification metrics:

- **Accuracy**: 78%
- **Precision, Recall, F1-Score**: Both models showed similar performance, with a slight advantage in precision for the non-diabetic class.

This indicates that feature scaling did not have a significant impact on the Logistic Regression model's performance in this case.

## Conclusion

The project showcases the application of Logistic Regression for binary classification. While feature scaling is a crucial step in many machine learning models, it had minimal effect in this specific case. The findings highlight the importance of understanding the data and model requirements before applying transformations.
