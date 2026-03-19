💳 Fraud Detection Using Imbalanced Data
📌 Overview

This project focuses on detecting fraudulent transactions using machine learning techniques on highly imbalanced data. The model is trained on transaction and identity datasets and uses feature engineering, dimensionality reduction, and classification to identify fraud patterns.

🚀 Features

Handles imbalanced dataset

Performs data preprocessing & cleaning

Uses feature selection (Top 10 important features)

Applies PCA (Principal Component Analysis) for dimensionality reduction

Trains an XGBoost Classifier

Evaluates model using:

Classification Report

Confusion Matrix

Deploys model using a Flask web application

🧠 Tech Stack

Python 🐍

Pandas, NumPy

Scikit-learn

XGBoost

Matplotlib & Seaborn

Flask

Joblib

📂 Dataset

The dataset used is from the IEEE Fraud Detection competition.

train_transaction.csv

train_identity.csv

👉 Note: Due to size restrictions, datasets are not included in this repository.

⚙️ Workflow
1. Data Preprocessing

Merged transaction & identity datasets

Dropped columns with excessive missing values

Filled remaining missing values

Encoded categorical features

2. Sampling

Randomly sampled 100,000 records for faster training

3. Feature Selection

Selected top 10 features based on correlation with target (isFraud)

4. Data Splitting

Train-test split (80/20)

5. Scaling

Applied StandardScaler

6. Dimensionality Reduction

Applied PCA (5 components)

7. Model Training

Used XGBoost Classifier

8. Evaluation

Classification Report

Confusion Matrix

📊 Visualizations

Fraud vs Non-Fraud distribution

Missing value analysis

Correlation heatmap

Feature distributions

Boxplots for fraud comparison

💾 Model Saving

The following files are saved using Joblib:

model.pkl

scaler.pkl

pca.pkl

features.pkl

🌐 Flask Web App
Run the App
python app.py
Access in Browser
http://127.0.0.1:5000/
Functionality

Input top 10 features manually

Predict whether a transaction is:

Fraud

Not Fraud

📁 Project Structure
├── notebook.ipynb
├── model.pkl
├── scaler.pkl
├── pca.pkl
├── features.pkl
├── app.py
└── README.md
📈 Future Improvements

Handle imbalance using:

SMOTE

Undersampling / Oversampling

Hyperparameter tuning

Deploy on cloud (AWS / Heroku)

Build a better UI (React / Streamlit)
