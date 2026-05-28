# Machine Learning Regression & Classification Projects

Welcome to my repository showcasing practical machine learning implementations using Python, Pandas, and Scikit-Learn. This repository focuses on end-to-end workflows, emphasizing data cleaning, exploratory data analysis (EDA), feature engineering, and model evaluation.

---

## 🚀 Project 1: Advertising Click-Through Rate (CTR) Prediction
**Goal:** Predict whether a user will click on an advertisement based on demographic factors and internet usage habits.

### 🧠 Data Engineering & Cleaning Highlights
* **Feature Selection:** Identified and dropped high-cardinality textual features (`Ad Topic Line`, `City`, `Country`) that would cause massive overfitting or unmanageable dimensionality during dummy encoding.
* **Text Processing:** Extracted structural meaning from raw strings and focused strictly on dense numerical behaviors.
* **Optimization Tuning:** Resolved algorithmic `ConvergenceWarning` flags by scaling optimizer parameters (`max_iter=1000`) to guarantee mathematical stability during gradient optimization.

### 📊 Model Performance (Logistic Regression)
The model achieved highly balanced metrics across both classes, proving its reliability for target marketing optimization:

* **Overall Test Accuracy:** 93%
* **Class 1 (Clicked) Precision:** 94% — Highly dependable targeting with minimal budget waste.
* **Class 1 (Clicked) Recall:** 90% — Successfully captured the vast majority of converting users.

---

## 🚢 Project 2: Titanic Survival Data Pipeline & Imputation
**Goal:** Clean and preprocess the classic Titanic dataset to prepare it for binary classification models.

### 🧠 Data Engineering & Cleaning Highlights
* **Smart Imputation:** Avoided lazy global averages for missing values. Instead, analyzed age distributions using boxplots and built a custom structural row-by-row factory function (`impute_age`) to patch missing `Age` values based on a passenger's socio-economic status (`Pclass`).
* **Dimensionality Management:** Permanently dropped data-scarce columns (`Cabin`) using explicit matrix targeting (`axis=1`).
* **Categorical Encoding:** Transformed textual categories into clean binary states (`0` and `1`) using `pd.get_dummies()` and verified execution state handling to prevent structural duplication errors in Jupyter's memory space.

---

## 🛠️ Tech Stack & Tools Used
* **Language:** Python
* **Environment:** Jupyter Notebook / Anaconda
* **Data Libraries:** Pandas, NumPy
* **Visualization:** Seaborn, Matplotlib
* **Machine Learning:** Scikit-Learn (Logistic Regression, Classification Metrics)

---

## 📈 Key Takeaways
Through these projects, I mastered the fundamental truth of data science: **"Garbage In, Garbage Out."** The vast majority of performance gains and model stability came directly from thorough exploratory data analysis, deliberate handling of missing values, and precise categorical engineering rather than just tuning the final classifier math.
