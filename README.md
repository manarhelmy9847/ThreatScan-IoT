# 🛡️ Multiclass IoT Attack Classifier

This project builds a machine learning model to classify different types of attacks targeting **Internet of Things (IoT)** networks. The goal is to detect and distinguish between various cyber threats using supervised learning techniques on labeled IoT traffic datasets.

---

## 🧠 Overview

The rapid expansion of IoT devices makes them attractive targets for cyberattacks. This classifier identifies multiple attack types (e.g. DoS, DDoS, MITM, PortScan, Botnet) using feature-engineered data from IoT traffic logs.

---

## 📂 Dataset

- **Source**: [BoT-IoT Dataset]
- **Classes**:  
  - 🟢 Normal  
  - 🔴 DoS  
  - 🟠 DDoS  
  - ⚫ Botnet  
  - 🟡 MITM  
  - 🔵 PortScan  

---

## ✨ Features

- Data preprocessing (cleaning, label encoding, scaling)
- Multiclass classification using:
  - Random Forest
  - XGBoost
  - KNN / SVM (optional)
- Evaluation metrics:
  - Accuracy, Precision, Recall, F1-score
  - Confusion matrix
- Feature importance analysis
- (Optional) Real-time prediction simulation

---

## 🛠️ Technologies Used

- Python 3.x  
- Scikit-learn  
- XGBoost / LightGBM  
- Pandas / NumPy  
- Matplotlib / Seaborn  
- Jupyter Notebook

---
