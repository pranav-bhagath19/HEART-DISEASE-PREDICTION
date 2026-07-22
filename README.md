# Heart Disease Prediction

A machine learning project for predicting the presence of heart disease using the K-Nearest Neighbors (KNN) classification algorithm.

## 📋 Overview

This project implements a classification model to predict whether a patient has heart disease based on various health metrics. The model is trained on a heart disease dataset and evaluated using accuracy metrics with different k-values to find optimal performance.

## 📊 Dataset

The project uses the **heart.csv** dataset containing medical and health information such as:
- Age
- Sex
- Chest pain type
- Blood pressure
- Cholesterol levels
- Maximum heart rate achieved
- And other relevant cardiac indicators

**Target Variable:** `HeartDisease` (binary classification: 0 or 1)

## 🛠️ Technologies & Libraries

- **Python 3.x**
- **pandas** - Data manipulation and analysis
- **scikit-learn** - Machine learning algorithms
  - `KNeighborsClassifier` - KNN model
  - `train_test_split` - Train-test split
  - `StandardScaler` - Data preprocessing
  - `accuracy_score` - Model evaluation

## 🔄 Workflow

1. **Data Loading** - Load heart disease data from CSV
2. **Exploratory Data Analysis (EDA)** - Examine data structure, info, statistics, and null values
3. **Data Preprocessing**
   - One-hot encoding of categorical variables
   - Feature-target separation
   - Train-test split (80-20)
   - Feature scaling using StandardScaler
4. **Model Training** - Train KNN classifier
5. **Model Evaluation** - Calculate accuracy and test k-values (1-20) for optimization

## 📈 Key Findings

The script evaluates KNN performance with k-values ranging from 1 to 20 to identify the optimal number of neighbors for accurate predictions.

## 🚀 Usage

Run the script with:

```bash
python heart_diesase.py
```

The script will:
- Load and analyze the dataset
- Train the KNN model
- Display predictions on test data
- Show accuracy scores
- Compare performance across different k-values

## 📁 Project Structure

```
HEART-DISEASE/
├── heart_diesase.py    # Main script
├── heart.csv           # Dataset
└── README.md           # Project documentation
```

## 📊 Model Details

- **Algorithm:** K-Nearest Neighbors (KNN)
- **Default k-value:** 5
- **Test size:** 20% of total data
- **Scaling:** StandardScaler for feature normalization
- **Metric:** Accuracy Score

## 📝 Notes

- The dataset is split into 80% training and 20% testing data
- Features are scaled before model training for better performance
- The script tests k-values from 1 to 20 to find the most accurate configuration

## 🎯 Future Improvements

- Implement cross-validation for more robust evaluation
- Compare with other classification algorithms (Logistic Regression, Decision Trees, etc.)
- Add feature importance analysis
- Create visualization plots for results
- Implement hyperparameter tuning

## 📄 License

This project is provided as-is for educational purposes.

---

**Last Updated:** 2026-07-22
