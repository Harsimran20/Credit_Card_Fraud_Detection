🚀 Credit Card Fraud Detection
📌 Table of Contents
Project Overview

Dataset

Installation

Usage

Model Overview

Results

📖 Project Overview
This project aims to detect fraudulent credit card transactions using machine learning classification techniques. It involves data preprocessing, feature engineering, and model evaluation to build a robust fraud detection system [6].

📂 Dataset
 The dataset contains 284,807 transactions with 31 features including:

Time: This shows how many seconds have passed since the first transaction in the dataset.
V1-V28: These are special features created to hide sensitive information about the original data.
Amount: Transaction amount.
Class: Target variable (0 for normal transactions, 1 for fraudulent transactions).

⚙️ Installation

git clone repository
cd credit-card-fraud-detection
pip install -r requirements.txt
▶️ Usage
To run the project:
python main.py
🧠 Model Overview
Algorithms used:

Logistic Regression

Random Forest

XGBoost

Evaluation metrics: Precision, Recall, F1-score, ROC-AUC.

📊 Results
The best model achieved an ROC-AUC score of 0.98, with high recall for fraudulent cases.

