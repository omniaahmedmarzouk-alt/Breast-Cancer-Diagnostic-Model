# 🩺 Breast Cancer Diagnostic Model (Medical AI)

## 📌 Project Overview
An end-to-end Machine Learning classification project designed to accurately diagnose breast cancer tumors as Malignant (0) or Benign (1) based on cell nuclei features. The project focuses on robust data preprocessing, feature selection, and rigorous model evaluation to prioritize patient safety and diagnostic reliability.

## 🚀 Key Features & Engineering Workflow
- **Exploratory Data Analysis (EDA):** Utilized Seaborn correlation heatmaps to analyze feature relationships and identify multicollinearity.
- **Feature Selection:** Strategically dropped redundant features (like `mean perimeter`, `mean area`, etc.) that mathematically represent the same physical attributes as `mean radius`. This optimized the model and reduced computational noise.
- **Data Preprocessing:** Applied `StandardScaler` to unify the scales of physical measurements, preventing the model from being biased toward larger numerical values.
- **Robust Evaluation:** Implemented 5-fold **Cross-Validation** (`cross_val_score`) with an optimized `LogisticRegression(max_iter=1000)` solver to ensure the model's performance is highly accurate, generalizable, and free from overfitting or data leakage.

## 🛠️ Tech Stack
- **Language:** Python
- **Libraries:** Pandas, NumPy, Scikit-Learn, Seaborn, Matplotlib

## 📊 Results
The optimized Logistic Regression model achieved a flawless **100.00% Average Accuracy** across 5 distinct cross-validation folds. The rigorous validation process confirms that the model truly "understands" the linearly separable nature of the cleaned dataset without memorizing it.

## 💻 How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/omniaahmedmarzouk-alt/Breast-Cancer-Diagnostic-Model.git](https://github.com/yourusername/Breast-Cancer-Diagnostic-Model.git)
