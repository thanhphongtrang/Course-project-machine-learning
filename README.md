# Supervised Learning for Human Activity Recognition

## Project Overview

This project aims to predict the manner in which participants perform a weightlifting exercise. The analysis is based on data collected from accelerometers on the belt, forearm, arm, and dumbbell of six participants. The goal is to build a machine learning model that can distinguish between the correct execution (Class A) and four common incorrect execution patterns (Classes B, C, D, and E).

This project is written in both R and Python

## Methodology

1.  **Data Preprocessing**: The raw training and testing datasets are loaded and inspected.
2.  **Feature Selection**: A multi-step feature selection process is applied to clean the data and remove irrelevant predictors:
    * Descriptive columns (timestamps, usernames) are removed.
    * Features with near-zero variance are eliminated.
    * Columns with a high percentage of missing values are dropped.
3.  **Model Training**: Two different supervised learning models are trained on the cleaned data:
    * **Random Forest Classifier**
    * **Support Vector Machine (SVM)**
4.  **Model Evaluation**: The models are evaluated on a validation set using accuracy and a confusion matrix to assess their performance.
5.  **Prediction**: The best-performing model (Random Forest) is used to predict the exercise quality for the final, unseen test set.

## Libraries Used in Python

* **`pandas`**: For data manipulation and loading.
* **`numpy`**: For numerical operations.
* **`scikit-learn`**: For data splitting, feature selection, modeling (Random Forest, SVM), and evaluation metrics.
* **`matplotlib` & `seaborn`**: For data visualization.

## How to Run

1.  Ensure you have Python and the libraries listed above installed.
2.  Place the `human_activity_recognition.ipynb` notebook in your project directory.
3.  Run the Jupyter Notebook cells sequentially to execute the analysis. The notebook will automatically download the required data.
