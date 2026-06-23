# SVM Classification Cancer Dataset

A machine learning project implementing Support Vector Machine (SVM) classification on cancer datasets for accurate disease diagnosis and prediction.

## 📋 Overview

This project demonstrates the application of Support Vector Machines (SVM) for binary classification of cancer types using the Cancer_Data.csv dataset. The implementation includes comprehensive data preprocessing, model training with cross-validation, and detailed performance evaluation metrics.

## 🎯 Objectives

- Load and explore cancer diagnostic data from the Cancer_Data.csv dataset
- Preprocess and normalize features for optimal SVM performance
- Train an SVM classifier on the cancer dataset
- Evaluate model performance using classification metrics
- Achieve high accuracy in cancer diagnosis prediction
- Compare training and testing accuracy to assess model generalization

## 📊 Dataset

**Dataset**: Cancer_Data.csv

The dataset includes:
- **Features**: 30 diagnostic measurements (radius, texture, perimeter, area, smoothness, compactness, concavity, etc.)
- **Target Variable**: `diagnosis` - Binary classification (Malignant vs. Benign)
- **Data Quality**: Includes an unnamed column (Unnamed: 32) which is removed during preprocessing
- **Class Distribution**: Imbalanced dataset with both malignant and benign cancer cases

## 🛠️ Technologies & Libraries

- **Python 3.x**
- **pandas**: Data loading and manipulation
- **scikit-learn**: 
  - SVM model implementation (SVC)
  - Train-test split for data partitioning
  - StandardScaler for feature normalization
  - Cross-validation for model robustness
  - Classification metrics (accuracy, confusion matrix, classification report)
- **Jupyter Notebook**: Interactive development environment

## 📈 Methodology

### Data Preprocessing
1. Load the cancer dataset using pandas
2. Check for missing values (null handling)
3. Remove unnecessary columns (Unnamed: 32)
4. Separate features (X) and target variable (y)
5. Analyze class distribution of diagnosis variable

### Data Splitting
- Split data into training (80%) and testing (20%) sets
- Use random_state=42 for reproducibility
- Maintain class distribution across train-test split

### Feature Scaling
- Apply StandardScaler to normalize all features
- Fit scaler on training data
- Transform both training and testing datasets
- Essential for SVM performance

### Model Training
- Instantiate Support Vector Classifier (SVC)
- Train on scaled training data
- Default kernel: RBF (Radial Basis Function)

### Model Evaluation
- Training set accuracy
- Testing set accuracy
- Confusion matrix analysis
- Detailed classification report with precision, recall, and F1-score

## 🔍 Key Features

- **Binary Classification**: Malignant vs. Benign cancer diagnosis
- **Feature Normalization**: StandardScaler ensures optimal SVM performance
- **Train-Test Validation**: Proper data splitting to prevent overfitting
- **Comprehensive Metrics**: Accuracy, precision, recall, F1-score, and confusion matrix
- **Classification Report**: Detailed performance breakdown per class

## 📊 Expected Results

The SVM model provides:
- **Training Accuracy**: High accuracy on training data
- **Testing Accuracy**: Reliable generalization to unseen data
- **Precision**: Measures false positive rate (important for cancer diagnosis)
- **Recall**: Measures false negative rate (critical to identify all cancer cases)
- **F1-Score**: Balanced metric combining precision and recall
- **Confusion Matrix**: Breakdown of true positives, true negatives, false positives, false negatives
uration & Customization

**Last Updated**: June 2026
