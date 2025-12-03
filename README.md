💧 Water Potability Prediction using Machine Learning

Predicting whether water is safe for drinking based on physicochemical properties using multiple machine learning models.

🚀 Project Overview

This project builds a machine learning system that predicts whether a given water sample is potable (safe to drink) or not.
It applies data preprocessing, imbalance handling, model training, hyperparameter tuning, and a Streamlit web interface for real-time predictions.

The goal is to support water quality monitoring and environmental safety using AI.

🧪 Dataset

The dataset used is the Water Potability dataset from Kaggle.
It contains 3,276 water samples with 9 chemical properties:

pH

Hardness

Solids

Chloramines

Sulfate

Conductivity

Organic Carbon

Trihalomethanes

Turbidity

Potability (Target)

🧹 Data Preprocessing

Handling missing values (mean/median imputation)

Scaling features using StandardScaler

Exploratory data analysis (distribution plots, heatmaps)

Outlier removal (IQR method)

Handling class imbalance using:

SMOTE (oversampling)

RandomUnderSampler (undersampling)

🧠 Machine Learning Models Used

Multiple classification models were trained and compared:

Model	Before Tuning	After Tuning
SVM (SVC)	✔	✔
Random Forest	✔	✔
K-Nearest Neighbors	✔	✔
Gradient Boosting	✔	✔
XGBoost	✔	✔
AdaBoost	✔	✔

Best performance was achieved using XGBoost + SMOTE.

📊 Model Evaluation Metrics

Accuracy

Precision

Recall

F1-score

ROC-AUC Curve

Confusion Matrix

These metrics were used to compare all models before and after tuning.

🌐 Web App (Streamlit)

A simple user-friendly web interface is created using Streamlit, where users can input water parameters and get the potability prediction instantly.

To run the app:
streamlit run project.py

🏗️ Project Structure
Water-Potability-Prediction/
│── data/
│── notebooks/
│── model/
│── project.py
│── requirements.txt
│── README.md
│── water_model.pkl

🛠️ Technologies Used

Python

Pandas, NumPy

Scikit-Learn

XGBoost

Imbalanced-learn (SMOTE)

Matplotlib, Seaborn

Streamlit

Pickle

📌 Key Features

End-to-end ML pipeline

Handles missing data & imbalance

Multiple ML models compared

Hyperparameter tuning

Streamlit prediction UI

Model saved using pickle

🎯 Results

The final deployed model achieved:

High accuracy

Improved recall for minority class

Robust predictions after tuning

📷 Screenshots
<img width="1891" height="865" alt="Screenshot 2025-11-28 160900" src="https://github.com/user-attachments/assets/30decdc7-ecae-41c9-a6c4-2b182578c805" />
