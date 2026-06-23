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

## 🚀 Getting Started

### Prerequisites
- Python 3.7 or higher
- pip or conda package manager

### Installation

1. Clone the repository:
```bash
git clone https://github.com/zaidkhan8241/SVM_Classification_Cancer_Dataset.git
cd SVM_Classification_Cancer_Dataset
```

2. Install required dependencies:
```bash
pip install -r requirements.txt
```

3. Create a virtual environment (optional but recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

## 📖 Usage

### Running the Classification Pipeline

1. **Place your dataset**:
   - Add `Cancer_Data.csv` to the project directory

2. **Run the Jupyter Notebook**:
   - Open `cancer_classification.ipynb` in Jupyter
   - Execute cells sequentially for step-by-step execution

3. **Key Execution Steps**:
   - Load and explore the cancer dataset
   - Perform exploratory data analysis (EDA)
   - Preprocess and scale features
   - Train the SVM model
   - Evaluate performance with detailed metrics

4. **View Results**:
   - Model accuracy scores
   - Classification report
   - Confusion matrix visualization

## 🎓 What You'll Learn

- Data preprocessing techniques for machine learning
- Feature scaling and normalization importance for SVM
- Train-test splitting methodology
- SVM classifier implementation and hyperparameters
- Model evaluation and interpretation of classification metrics
- Handling imbalanced datasets in medical diagnosis

## 🔧 Configuration & Customization

Potential enhancements:
- Experiment with different SVM kernels (linear, polynomial, sigmoid)
- Tune hyperparameters (C, gamma) using GridSearchCV
- Implement cross-validation for robust model evaluation
- Compare SVM with other classifiers (Random Forest, Logistic Regression)
- Handle class imbalance with class weights
- Perform feature selection to improve model interpretability

## 📁 Project Structure

```
SVM_Classification_Cancer_Dataset/
├── README.md
├── cancer_classification.ipynb
├── Cancer_Data.csv
└── requirements.txt
```

## 📦 Dependencies

Key packages:
- pandas >= 1.0.0
- scikit-learn >= 0.24.0
- numpy >= 1.19.0
- jupyter (for notebook development)

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -m 'Add enhancement'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Open a Pull Request

## 📝 License

This project is open source and available under the MIT License.

## 👤 Author

**Zaid Khan**
- GitHub: [@zaidkhan8241](https://github.com/zaidkhan8241)

## 🙏 Acknowledgments

- scikit-learn team for excellent machine learning tools
- Cancer dataset providers and medical researchers
- Open-source community for best practices and resources

## 📧 Contact & Support

For questions, issues, or suggestions:
- Open an [Issue](https://github.com/zaidkhan8241/SVM_Classification_Cancer_Dataset/issues)
- Submit a [Pull Request](https://github.com/zaidkhan8241/SVM_Classification_Cancer_Dataset/pulls)

## 📚 Further Reading

- SVM Theory and Implementation
- Feature Scaling in Machine Learning
- Medical Data Classification Best Practices
- Cancer Diagnosis Using Machine Learning

---

**Last Updated**: June 2026
