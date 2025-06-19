# Elevate-labs-task-7
Breast Cancer Classification using SVM

## 🔍 Objective
This project demonstrates the use of **Support Vector Machines (SVM)** for binary classification (malignant vs benign tumors) using the Breast Cancer Wisconsin dataset.

## 📂 Dataset
Source: 'breast-cancer.csv'
Target column: 'diagnosis'
 'M' = Malignant (1)
 'B' = Benign (0)

## 🛠 Tools & Libraries
- Python
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

## 📌 Key Concepts Covered
- Margin Maximization
- Kernel Trick (Linear & RBF)
- Hyperparameter Tuning with `GridSearchCV`
- Cross-validation for performance estimation
- PCA-based 2D Decision Boundary Visualization

## 🚀 Implementation Steps
1. **Data Preprocessing**
   - Dropped unnecessary `id` column
   - Encoded `diagnosis` column
   - Scaled features using `StandardScaler`

2. **Model Training**
   - SVM with Linear Kernel
   - SVM with RBF Kernel

3. **Visualization**
   - Used PCA to reduce dimensions to 2
   - Plotted decision boundaries

4. **Hyperparameter Tuning**
   - Used `GridSearchCV` to find optimal `C` and `gamma`

5. **Evaluation**
   - Accuracy, Confusion Matrix, Cross-validation scores

## 📈 Results

| Kernel | Accuracy |
|--------|----------|
| Linear | ~96%     |
| RBF    | ~98%     |

- Best Params from GridSearchCV: `{'C': 10, 'gamma': 0.01, 'kernel': 'rbf'}`
- Mean CV Score: ~98.2%
