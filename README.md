# Breast Cancer Classification with K-Nearest Neighbors

This Jupyter Notebook demonstrates a basic machine learning pipeline for classifying breast cancer using the K-Nearest Neighbors (KNN) algorithm. The goal is to predict whether a tumor is malignant or benign based on various features extracted from digitized images.

## Dataset

The project uses the **Breast Cancer Wisconsin (Diagnostic) Dataset**, which is a classic dataset for binary classification tasks. It contains 569 instances with 30 numeric, predictive features computed from a digitized image of a fine needle aspirate (FNA) of a breast mass. The target variable indicates whether the mass is malignant (cancerous) or benign (non-cancerous).

## Project Steps

The notebook covers the following steps:

1.  **Data Loading**: The `load_breast_cancer` function from `sklearn.datasets` is used to load the dataset.
2.  **Data Splitting**: The dataset is split into training and testing sets using `train_test_split` to evaluate the model's performance on unseen data.
3.  **Model Training**: A K-Nearest Neighbors (`KNeighborsClassifier`) model is initialized and trained on the training data.
4.  **Prediction**: The trained model makes predictions on the test set.
5.  **Model Evaluation**: The model's performance is evaluated using:
    *   A **Confusion Matrix**: Visualizing the true positives, true negatives, false positives, and false negatives. The model produced a confusion matrix of `[[ 78   5], [  5 140]]`, indicating 78 true negatives, 140 true positives, and 5 false positives, and 5 false negatives.
    *   A **Classification Report**: Providing precision, recall, f1-score, and support for each class. The model achieved an overall accuracy of 96%, with high precision (0.94-0.97) and recall (0.94-0.97) for both malignant and benign classes.

## Technologies Used

*   **Python**
*   **scikit-learn**: For machine learning functionalities (dataset loading, model selection, model training, and evaluation metrics).

## How to Run

1.  **Clone the repository** (once you have it on GitHub).
2.  **Open the notebook** in a Jupyter environment (e.g., Google Colab, Jupyter Lab, Jupyter Notebook).
3.  **Run all cells** sequentially. The output will display the data characteristics, model predictions, and evaluation metrics.
