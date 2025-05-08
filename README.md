# 🧠 Significant Feature Selection and Optimized Tumor Prediction

This project analyzes the **Wisconsin Diagnostic Breast Cancer (WDBC)** dataset to identify significant cellular features that best predict whether a tumor is benign or malignant. Using **statistical techniques** and **machine learning models**, we evaluate classification performance across several algorithms and compare results.

---

## 📊 Dataset Overview

- **Source**: UCI Machine Learning Repository (WDBC)
- **Observations**: 569 patient records
- **Attributes**: 32 (ID, Diagnosis, and 30 cell feature measurements)
- **Diagnosis**: Binary classification (M = Malignant, B = Benign)

---

## 🔍 Key Techniques Used

### 🧪 Feature Selection
- Exploratory Data Analysis (boxplots, histograms)
- Correlation heatmaps
- **t-tests** to compare benign vs malignant groups
- **Multicollinearity removal** using **VIF analysis**

### 🧠 Modeling Approaches
- **Logistic Regression** with backward selection
- **Decision Tree**
- **Random Forest** (with feature importance analysis)
- **K-Nearest Neighbors (KNN)** (optimized `k` via cross-validation)
- **Support Vector Machine (SVM)** (with kernel tuning and hyperparameter optimization)

### 📈 Evaluation Metrics
- Accuracy
- Precision
- Recall
- Confusion Matrix
- ROC Curves (for RF)
- Model comparison chart

---

## 🥇 Results

| Model           | Accuracy | Key Notes |
|----------------|----------|-----------|
| Decision Tree  | 91.76%   | Simple, interpretable |
| Random Forest  | 97.06%   | Best overall; high AUC |
| KNN (k=5)       | 95.88%   | Slight drop in sensitivity |
| SVM (linear)   | 97.06%   | Best for balanced precision/recall |

---

## 🛠️ Technologies Used

- **R** / RStudio
- Libraries: `caret`, `e1071`, `randomForest`, `class`, `car`, `ggplot2`
- Data visualization: ROC curve, variable importance, boxplots, correlation heatmap

---

## 📁 Repository Structure

├── Final_Project.Rmd # RMarkdown source file
├── Final_Project.pdf # PDF output with full analysis
├── STAT 385 Final Project Presentation.pdf
├── wdbc.data # Raw dataset
├── wdbc.names # Attribute documentation
├── .RData / .Rhistory # RStudio session files
└── README.md # This file

---

## 📌 Takeaway

This project shows how combining **feature engineering**, **statistical analysis**, and **machine learning** yields highly accurate tumor classification. It demonstrates the importance of model interpretability, multicollinearity mitigation, and thoughtful model selection.

---

## 📎 Related Links

- 📂 Dataset: [WDBC @ UCI ML Repo](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic))
- 💻 GitHub: [View Code](https://github.com/mohammadnusairat/Significant-Feature-Selection-and-Optimized-Tumor-Prediction)
