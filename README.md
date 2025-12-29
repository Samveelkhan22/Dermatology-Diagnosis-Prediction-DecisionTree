# Dermatology Diagnosis Prediction using Decision Tree

## 📌 Project Overview
This project focuses on building a **machine learning–based clinical decision support system** to predict dermatological diagnoses using patient clinical and histopathological features.  
A **Decision Tree classifier** is trained to classify skin conditions based on attributes such as erythema, scaling, itching, and microscopic tissue characteristics.

The goal is to demonstrate how **interpretable machine learning models** can assist healthcare professionals in improving diagnostic accuracy.

---

## 🧠 Problem Statement
Can dermatological diagnoses be accurately predicted using structured clinical and histopathological data?

Skin diseases such as psoriasis, eczema, and other inflammatory conditions affect millions worldwide. Early and accurate diagnosis is critical for effective treatment. This project frames dermatology diagnosis as a **multi-class classification problem** and applies supervised learning techniques to solve it.

---

## 📊 Dataset Description
- **Source:** UCI Machine Learning Repository – Dermatology Dataset  
- **Samples:** 366 patient records  
- **Features:** 34 clinical and histopathological attributes  
- **Target Variable:** `diagnosis` (6 distinct skin disease classes)

### Feature Types
- Clinical features: erythema, scaling, itching, family history
- Histopathological features: fibrosis, acanthosis, spongiosis, granular layer
- Demographic feature: age

---

## 🔍 Exploratory Data Analysis (EDA)
Key steps performed:
- Dataset inspection and summary statistics
- Missing value handling (median imputation for age)
- Target class distribution analysis
- Feature correlation analysis
- Visualization using:
  - Histograms
  - Box plots
  - Correlation heatmaps

EDA revealed **class imbalance** and identified **highly informative features** correlated with diagnosis.

---

## ⚙️ Data Preprocessing
- Missing values handled using median imputation
- Feature selection based on correlation threshold
- Train–test split (80/20) with stratification
- Feature standardization using `StandardScaler`

---

## 🌲 Model Selection: Decision Tree Classifier
A Decision Tree was chosen due to:
- High interpretability (critical for medical applications)
- Ability to capture non-linear relationships
- No requirement for feature scaling
- Robustness to noisy data

### Hyperparameters Tuned
- `max_depth`
- `min_samples_split`
- `min_samples_leaf`
- `max_features`

Hyperparameter tuning was performed using **GridSearchCV with 5-fold cross-validation**.

---

## 📈 Model Performance

### Initial Model
- **Accuracy:** 85.14%

### Tuned Model
- **Accuracy:** 83.78%
- **Cross-validation Mean Accuracy:** ~84.9%

### Evaluation Metrics
- Precision, Recall, and F1-score for each class
- Confusion matrix visualization
- Strong performance for majority classes
- Slight performance drop for underrepresented classes

---

## 🧪 Key Results
- Certain diagnoses achieved near-perfect precision and recall
- Class imbalance affected recall for some categories
- Model generalizes well based on cross-validation
- Interpretability makes it suitable for clinical insights

---

## ⚠️ Limitations
- Class imbalance impacts minority class performance
- Decision Trees may overfit without careful tuning
- Dataset size limits generalization
- Clinical deployment would require validation with real-world data

---

## 🚀 Future Improvements
- Use ensemble methods (Random Forest, Gradient Boosting)
- Apply class imbalance techniques (SMOTE, class weighting)
- Feature engineering and dimensionality reduction
- Model explainability using SHAP or LIME
- Compare performance with SVM and Neural Networks

---

## 🛠️ Technologies Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

---


---

## 📜 Disclaimer
This project is for **educational and research purposes only** and is not intended for clinical diagnosis or treatment.

---

## 👤 Author
**Samveel Zaheer Khan**  


## 📂 Project Structure
