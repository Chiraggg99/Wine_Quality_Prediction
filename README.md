# 🍷 Wine Quality Prediction using Random Forest

## 📌 Overview
This project implements a **Random Forest Classifier** to predict the quality of wine based on various chemical and physicochemical properties. The goal is to build a robust classification model that can assist in automating wine quality assessment, which traditionally relies on human tasting.

---

## 📊 Dataset

The dataset is sourced from the **UCI Machine Learning Repository** and contains **red wine samples**. Each row represents a wine sample with the following features:

### 🔬 Features:
- **Fixed Acidity** – Tartaric acid content
- **Volatile Acidity** – Acetic acid content (high levels cause vinegar taste)
- **Citric Acid** – Acts as a preservative
- **Residual Sugar** – Amount of sugar remaining after fermentation
- **Chlorides** – Salt content
- **Free Sulfur Dioxide** – Prevents microbial growth
- **Total Sulfur Dioxide** – Sum of free and bound forms
- **Density** – Related to sugar and alcohol content
- **pH** – Acidity level
- **Sulphates** – Additive contributing to sulfur dioxide levels
- **Alcohol** – Alcohol content in % volume
- **Quality (Target)** – Score between 0 and 10 (based on sensory data)

## 🧠 Model & Approach

### 🔍 Exploratory Data Analysis (EDA)
- **Visualized feature distributions** using Seaborn histograms and KDE plots.
- **Plotted correlations** with a heatmap to identify strongly related features.
- Detected **outliers** and **missing values** (if any).
- Boxplots and scatterplots used to understand relationships with the target.

### ⚙️ Feature Engineering
- Applied **MinMaxScaler** to normalize features.
- Converted the **'quality'** variable into categorical labels (optional step).
- Handled **class imbalance** by analyzing distribution of quality scores.

### 🌲 Machine Learning Model
- Implemented a **Random Forest Classifier** from scikit-learn.
- Performed **hyperparameter tuning** 
- Used **train_test_split** for model validation.

### 📈 Evaluation Metrics
- **Accuracy**: Overall correctness
- **Precision & Recall**: For each class
- **F1-Score**: Harmonic mean of precision and recall
- **Confusion Matrix**: For visualizing misclassifications
- **Feature Importance**: Determined which features influenced predictions most

📌 Model achieved an accuracy of approximately **92.6%** 

---

## ⚙️ Installation & Requirements

Make sure you have Python 3.x installed. Then install the following packages:

```bash
pip install numpy pandas scikit-learn seaborn matplotlib

