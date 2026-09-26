# 🧠 Social Media & Digital Wellbeing: Mental State Classification 📱✨

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg?logo=python&logoColor=white)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg?logo=jupyter&logoColor=white)](https://jupyter.org)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E.svg?logo=scikit-learn&logoColor=white)](https://scikit-learn.org)
[![Status](https://img.shields.io/badge/Project-Complete-brightgreen.svg)]()

> An end-to-end Machine Learning project exploring the correlation between daily screen time, social media habits, lifestyle factors, and mental wellbeing.

---

## 📌 Project Overview 🎯

With increasing reliance on digital devices, screen time and social interactions have a profound effect on mental wellness[cite: 2]. This project implements a full machine learning pipeline—from exploratory data analysis (EDA) to multi-class classification—predicting an individual's mental state (`Healthy`, `Stressed`, `At_Risk`).

### 🔍 Key Highlights:
- 📊 **Exploratory Data Analysis (EDA):** Analyzed behavioral trends, platform usage, and distribution of stress/anxiety levels.
- 📉 **Dimensionality Reduction:** Evaluated performance before and after applying **Principal Component Analysis (PCA)**.
- 🤖 **Model Benchmarking:** Compared four machine learning algorithms across Accuracy, Precision, Recall, and F1-score.
- 📈 **Performance Visualization:** Confusion matrices, accuracy comparisons, and multi-class One-vs-Rest ROC/AUC curves.

---

## 🗂️ Dataset Features 📋

The dataset captures demographic, digital engagement, and lifestyle indicators:

| Feature Category | Features Included |
| :--- | :--- |
| **Demographics** 👤 | Age, Gender |
| **Digital Usage** 📱 | Platform (Instagram, Snapchat, YouTube, etc.), Daily Screen Time (mins), Social Media Time (mins) |
| **Social Sentiment** 💬 | Positive Interactions Count, Negative Interactions Count |
| **Lifestyle & Vitals** 🏃‍♂️ | Sleep Hours, Physical Activity (mins) |
| **Psychological Levels** 🧠 | Anxiety Level, Stress Level, Mood Level |
| **Target Variable** 🎯 | **`mental_state`** (`Healthy` / `Stressed` / `At_Risk`) |

---

## 🔬 Machine Learning Pipeline ⚙️

1. **Preprocessing & Scaling:** Handled missing values, categorical encoding, and feature standardization via `StandardScaler`.
2. **Feature Extraction:** Transformed high-dimensional feature spaces using **PCA** to assess dimensionality trade-offs.
3. **Classifiers Tested:**
   - 🌲 **Random Forest** (Best Performing)
   - 📈 **Logistic Regression**
   - ⚡ **Support Vector Machine (SVM - RBF Kernel)**
   - 📍 **K-Nearest Neighbors (KNN)**
4. **Evaluation:** Evaluated with 5-fold cross-validation, weighted F1-scores, and multiclass ROC-AUC metrics.

---

## 📊 Experimental Results 🏆

### 📈 Model Accuracy: Original Features vs. PCA

| Model | Original Data (Accuracy) | PCA Transformed (Accuracy) | Best Space |
| :--- | :---: | :---: | :---: |
| 🌲 **Random Forest** | **1.000** | **0.996** | **Original** |
| 📈 **Logistic Regression** | **0.995** | **0.987** | **Original** |
| ⚡ **SVM (RBF)** | **0.987** | **0.986** | **Original** |
| 📍 **KNN** | **0.981** | **0.979** | **Original** |

> 💡 **Key Takeaway:** Tree-based ensemble learning (**Random Forest**) achieved near-perfect classification on both original and reduced feature spaces. Retaining the full feature set yielded slightly superior performance across all benchmarks.
---

## 🚀 Getting Started 💻

### 1️⃣ Clone the Repository
```bash
git clone [https://github.com/Sammy6899/SocialMedia-mental-health-ml-classification.git](https://github.com/Sammy6899/SocialMedia-mental-health-ml-classification.git)
cd SocialMedia-mental-health-ml-classification
```

### 2️⃣ Set Up a Virtual Environment & Install Dependencies
```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

### 3️⃣ Run the Notebook
```bash
jupyter notebook Project437.ipynb
```

> ☁️ *Or upload directly to [Google Colab](https://colab.research.google.com/) for cloud execution!*

---

## 📦 Core Dependencies 🛠️

- `python >= 3.8`
- `pandas`[cite: 1, 2]
- `numpy`[cite: 1]
- `scikit-learn`[cite: 1]
- `matplotlib`[cite: 1, 2]
- `seaborn`[cite: 2]

---

## 🤝 Contributing & License 📜

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/Sammy6899/SocialMedia-mental-health-ml-classification/issues).

Distributed under the **MIT License**. See `LICENSE` for more information.
