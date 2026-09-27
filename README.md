# 🧠 Social Media Usage and Mental Health Prediction:
A Machine Learning Classification Study
 📱✨

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg?logo=python&logoColor=white)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg?logo=jupyter&logoColor=white)](https://jupyter.org)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E.svg?logo=scikit-learn&logoColor=white)](https://scikit-learn.org)
[![Status](https://img.shields.io/badge/Project-Complete-brightgreen.svg)]()

> An end-to-end Machine Learning project exploring the correlation between daily screen time, social media habits, lifestyle factors, and mental wellbeing.

---

## 📄 Research Paper

This repository contains the official dataset, experimental code, and pipeline for the research study:

> **"Social Media Usage and Mental Health Prediction: A Machine Learning Classification Study"**  
> *Nafiz Ahmed, Samiha Tasnim Orthi, Maimuna Morshed, Safiur Rahman Safi*  
> Department of Computer Science & Engineering, BRAC University, Dhaka, Bangladesh[cite: 12]  
> 📖 **[Read the Full Paper (PDF)](docs/CSE437_IEEE_Conference_Paper.pdf)**[cite: 12]

### 📝 Abstract Summary
Operating on 5,000 multi-platform behavioral records across seven platforms (Facebook, TikTok, YouTube, WhatsApp, Snapchat, Instagram, and Twitter), this study designs an expanded 45-predictor feature engineering matrix[cite: 12]. Benchmarking four classifiers (Random Forest, Logistic Regression, Support Vector Machine, and K-Nearest Neighbors) demonstrates that Random Forest achieves perfect classification ($Accuracy = F1 = 1.000$) on the original feature space[cite: 12]. Furthermore, a 64.4% dimensionality reduction via Principal Component Analysis (retaining 16 components with 95.93% variance) incurs at most a 0.5% degradation across all models, proving that digital behavioral metadata carries compact, highly discriminative signals regarding psychological state[cite: 12].

---

## 📌 Project Overview 🎯

With increasing reliance on digital devices, screen time and social interactions have a profound effect on mental wellness. This project implements a full machine learning pipeline—from exploratory data analysis (EDA) to multi-class classification—predicting an individual's mental state (`Healthy`, `Stressed`, `At_Risk`).

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
jupyter notebook mental_health_ml_classification.ipynb
```

> ☁️ *Or upload directly to [Google Colab](https://colab.research.google.com/) for cloud execution!*

---

## 📦 Core Dependencies 🛠️

- `python >= 3.8`
- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `seaborn`

---

## 👤 Author & Acknowledgments

- **Developer:** [Sammy6899](https://github.com/Sammy6899)
- **Course:** CSE437 - Data Science
