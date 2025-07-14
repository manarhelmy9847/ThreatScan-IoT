# 🛡️ Multiclass IoT Attack Classifier

This project presents a machine learning model designed to classify multiple types of cyberattacks targeting Internet of Things (IoT) devices. Using real-world traffic data from the **N-BaIoT dataset**, the model aims to detect malware families like **Mirai** and **Gafgyt**, which are known for launching large-scale IoT-based attacks.

---

## 🎯 Objective

To develop a robust multiclass classification system capable of detecting various IoT botnet attacks using supervised learning—supporting 11 classes (10 attack types + 1 benign class).

---

## 📊 Dataset: N-BaIoT

- **Samples:** ~7 million records  
- **Features:** 115 numerical network traffic features  
- **Devices:** Data collected from 9 real infected IoT devices  
- **Classes:** 11 total (benign + 10 attack types like `gafgyt_udp`, `mirai_scan`, etc.)

---

## 🔧 Preprocessing

1. **Label Encoding:** All textual labels (e.g., `mirai_udp`, `benign`) were encoded as integers.
2. **Resampling:** Balanced the dataset by sampling 100 examples per class to prevent model bias.
3. **Train-Test Split:** 60% for testing, 40% for training across all classes.
4. **Feature Analysis:** Statistical measures (mean, std, correlation) were used to understand feature relevance.

---

## 🤖 Model: XGBoost Classifier

- Chosen for its high performance on structured data.
- Supports native multiclass classification.
- Handles class imbalance well.
- Implements pruning and regularization to prevent overfitting.

---

## 🧪 Evaluation

- **Accuracy:** Over **98%**  
- **Classification Report:** High precision, recall, and F1-score across all classes  
- **Confusion Matrix:** Shows minimal confusion even between similar attack types (e.g., `mirai_udp` vs `mirai_udpplain`)

---

## 📌 Conclusion

The classifier successfully distinguishes between multiple IoT attack types, even with limited data per class. The model serves as a foundation for developing a lightweight **Intrusion Detection System (IDS)** for smart environments and can be improved with:

- Hyperparameter tuning  
- Deep learning & time-series models  
- Explainable AI techniques

---

