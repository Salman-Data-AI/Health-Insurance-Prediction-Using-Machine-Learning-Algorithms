# Health Insurance Lead Prediction Using Machine Learning

This project presents a comprehensive machine learning pipeline to predict whether a customer is likely to respond positively to a health insurance offer, based on their profile and historical behavior. It is built using Python, with experiments conducted on Google Colab using a Kaggle dataset.

![image](https://github.com/user-attachments/assets/d5d9c5da-d57f-42d8-ad6a-1c323efd1290)

---

## 📌 Problem Statement

The goal is to assist banks in identifying which existing customers are most likely to opt-in for cross-sold health insurance products, thereby increasing revenue per customer while minimizing campaign costs.

---

## General Architecture

![image](https://github.com/user-attachments/assets/a0d22eca-69b3-4648-8a25-2ab584dca73e)

---

## 🧠 Machine Learning Approach

We adopted a multi-phase model experimentation strategy:
- **Data Cleaning & Outlier Removal** using IQR
- **Feature Encoding** (One-Hot and Label Encoding)
- **Scaling** using Min-Max Normalization
- **Dimensionality Reduction** using PCA
- **Model Benchmarking** using LazyPredict
- **Deep Learning Model** with CNN architecture
- **Hyperparameter Tuning** with RandomizedSearchCV

---

## Process Diagram

![image](https://github.com/user-attachments/assets/46cd22fe-064e-419f-9091-9adfca7a0808)

---

## 🔍 Dataset

- Source: [Kaggle Health Insurance Lead Prediction Dataset](https://www.kaggle.com/competitions/health-insurance-cross-sell-prediction/data)
- Size: 50,000+ records
- Target Variable: `Response` (0 = No, 1 = Yes)

---

## 📈 Model Evaluation Metrics

- **Accuracy**
- **ROC-AUC**
- **Precision / Recall**
- **Confusion Matrix**

The final model was chosen based on balanced accuracy and AUC score with special emphasis on recall for positive (opt-in) predictions.

---

## Solution Architecture

![image](https://github.com/user-attachments/assets/e1f2df66-2e77-4068-b455-bd504460d7c5)

--

## 📁 Project Structure

- `Health_Insurance_Lead_Prediction_Project.ipynb` – Core Google Colab notebook with full EDA, preprocessing, and modeling
- `Thesis.pdf` – Complete academic dissertation documenting methodology, model comparisons, and results
- `train.csv` – Dataset used for training (external Kaggle data, not uploaded)

---

## 🛠️ Tools Used

- Python (Pandas, NumPy, Scikit-learn, TensorFlow, Keras, LazyPredict)
- Google Colab
- Matplotlib & Seaborn (for visualizations)
- Azure & Informatica (mentioned in real-world deployment context)

---

## 🏁 Results Summary

- CNN and tree-based models like XGBoost achieved the highest classification performance.
- Careful treatment of outliers and missing values contributed to model robustness.
- The final solution is designed to be deployable within an enterprise DWH + ML Ops setup using cloud tools.

### Correlation Matrix

![image](https://github.com/user-attachments/assets/ca092e80-6b8a-4402-8a29-1bb7782550b2)

---

### Confusion Matrix

![image](https://github.com/user-attachments/assets/ad7b045e-e3f7-4ff7-ad58-bd08fe3a5995)

---

## 📚 References

- [BITS Pilani M.Tech Dissertation 2023](https://bits-pilani.ac.in)
- Kaggle Notebooks and Public Leaderboards

---

## 📬 Author

**Salman Khan**  
M.Tech, BITS Pilani  

---

⭐ *If you find this project useful, feel free to star this repo!*
