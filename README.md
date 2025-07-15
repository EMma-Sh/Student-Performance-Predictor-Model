# 🎓 Student Performance Predictor

A machine learning project that predicts whether a student will pass or fail based on academic, personal, and social features. This project uses supervised learning techniques to build and evaluate classification models on the UCI Student Performance Dataset.

## 🎯 Goal

To build a binary classification model that predicts a student's final result (pass/fail) using features such as study time, family background, health, and prior grades.

## 🧰 Tools & Technologies

- **Python**
- **Pandas, NumPy** – Data preprocessing
- **Scikit-learn** – Model training & evaluation
- **Matplotlib, Seaborn** – Visualization

## 📂 Dataset

- **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/student+performance)
- **Files Used**: `StudentData.csv` (Math course)
- **Features Include**:
  - Demographics (age, gender, address)
  - Education-related (study time, absences)
  - Family (parent education, support)
  - Grades (G1, G2, G3)

## ⚙️ Steps Performed

1. **Data Cleaning**: Handled missing values, cleaned column names
2. **Feature Engineering**: Created binary target (`pass`) based on G3 ≥ 10
3. **Encoding**: Converted categorical columns using one-hot encoding
4. **Train/Test Split**: 80/20 split using `train_test_split`
5. **Scaling**: Standardized numerical features with `StandardScaler`
6. **Model Training**:
   - Logistic Regression
   - Decision Tree Classifier
7. **Evaluation**:
   - Accuracy, Precision, Classification Report
   - Confusion Matrix
8. **Feature Importance**: Identified key predictors using tree-based model
   
## 📊 Results

| Model              | Accuracy | Precision |
|-------------------|----------|-----------|
| Logistic Regression | ~0.80    | ~0.82     |
| Decision Tree       | ~0.78    | ~0.80     |

✅ Decision Tree helped in understanding **which features** (like prior grades, study time, family support) most affect the chances of passing.

## 🧠 Key Insights

- Students with **higher G1 & G2 scores** are far more likely to pass.
- **Study time**, **parental support**, and **absence rate** have noticeable impact.
- Decision Trees provide better interpretability, while Logistic Regression gives stable performance.

**Eman Iqbal**  
Final Year Computer Science Student  
📍 Pakistan  
📧 emmnqb@gmail.com  
🔗 www.linkedin.com/in/  

## 📌 Future Improvements

- Hyperparameter tuning for decision tree
- Try ensemble models (Random Forest, XGBoost)
- Use both math and Portuguese datasets together
- Build an interactive dashboard using Streamlit

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).
