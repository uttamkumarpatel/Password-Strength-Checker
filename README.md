🔐 NLP-based Password Strength Checker

This project implements a **Password Strength Checker** using **Natural Language Processing (NLP)** and **Machine Learning** techniques. It classifies passwords into strength categories (weak, medium, strong) and provides insights on password security.

---

## 📌 Project Overview

* Dataset: \~100,000 leaked passwords (000webhost leak).
* Labels: Passwords were categorized into strength levels.
* Feature Engineering:

  * **TF-IDF Vectorization** to represent passwords numerically.
  * Sparse matrix representation with \~99 features per password.
* Model: **Logistic Regression** trained on TF-IDF features.
* Evaluation:

  * Accuracy and **Weighted F1-score \~77%**.
  * Balanced evaluation of weak/medium/strong categories.
* Goal: Detect weak/common passwords and encourage stronger password practices.

---

## 🛠️ Tech Stack

* **Python**
* **scikit-learn** (Logistic Regression, TF-IDF Vectorizer)
* **pandas, NumPy**
* **Matplotlib, Seaborn** (visualization)
* **Jupyter Notebook**

---

## 📊 Results

* The model successfully learns password strength patterns.
* TF-IDF features capture character sequences effectively.
* Weak and strong passwords are classified well; medium passwords are harder due to overlap.
* Achieved a **weighted F1-score of \~0.77**.

---

## 🚀 How to Run

1. Clone this repository:

   ```bash
   git clone https://github.com/uttamkumarpatel/Password-Strength-Checker.git
   cd Password-Strength-Checker
   ```
2. Install dependencies:

3. Open the Jupyter Notebook:

   ```bash
   jupyter notebook NLP_password_strength_Uttam_Kumar.ipynb
   ```
4. Run all cells to reproduce results.

---

## 📂 Repository Structure

```
Password-Strength-Checker/
│── NLP_password_strength_Uttam_Kumar.ipynb   # Main notebook
│── password_data.sqlite                      # Dataset (local storage)
                 
```

---

## 🔮 Future Work

* Add a **Streamlit app** for interactive password strength checking.
* Explore **deep learning (LSTMs / Transformers)** for sequence modeling.
