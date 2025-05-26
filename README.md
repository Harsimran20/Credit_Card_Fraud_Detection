
# 🚀 Credit Card Fraud Detection

📌 **Table of Contents**
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Model Overview](#model-overview)
6. [Results](#results)
7. [License](#license)

---

## 📖 Project Overview

Credit card fraud detection is a critical challenge in the financial sector. This project aims to build a machine learning pipeline that accurately detects fraudulent transactions using real-world data. It includes:
- Exploratory data analysis (EDA)
- Data preprocessing and balancing
- Feature selection and engineering
- Model training and evaluation
- Performance visualization

The goal is to identify fraud in a highly imbalanced dataset with a focus on minimizing false negatives.

---

## 📂 Dataset

 The dataset contains 284,807 transactions with 31 features including:

Time: This shows how many seconds have passed since the first transaction in the dataset.
V1-V28: These are special features created to hide sensitive information about the original data.
Amount: Transaction amount.
Class: Target variable (0 for normal transactions, 1 for fraudulent transactions).

### Features:
- `Time`: Time in seconds since the first transaction
- `V1` to `V28`: PCA-transformed features to protect confidentiality
- `Amount`: Purchase amount
- `Class`: Target variable (0 = legitimate, 1 = fraud)

The data is highly imbalanced, which poses a challenge for model performance.

---

## ⚙️ Installation

To set up the project environment, run:

```bash
git clone repository
cd credit-card-fraud-detection
pip install -r requirements.txt
```

---

## ▶️ Usage

To execute the full pipeline:

python main.py

Output metrics and visualizations will be stored in the `/outputs` directory.

---

## 🧠 Model Overview

This project experiments with several machine learning algorithms:

- **Logistic Regression**: A baseline linear model
- **Random Forest**: Ensemble of decision trees for improved performance
- **XGBoost**: Gradient boosting model for high accuracy
- **Isolation Forest**: Anomaly detection algorithm for unsupervised scenarios
- **SMOTE**: Applied for oversampling the minority class to address imbalance

Evaluation metrics include:
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC Curve

---

## 📊 Results

- **Random Forest** achieved a recall of **0.92**, balancing detection rate with low false positives.
- **XGBoost** had the best overall F1-score.
- Confusion matrices and ROC curves are provided in `/plots`.

---

## 📄 License

This project is licensed under the MIT License. See `LICENSE` for more details.

