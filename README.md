# Restaurant-Revenue-Prediction
This project uses **regression, classification, and resampling methods** to analyze a simulated restaurant dataset and predict monthly revenue. The aim is to identify the most important business factors contributing to a restaurant’s financial success, using both exploratory data analysis and advanced modeling techniques.

---

## 🎯 Project Goals

- Predict restaurant revenue using marketing, customer, and menu data
- Classify restaurants into success levels based on profitability
- Compare performance of multiple predictive models including linear regression, QDA, LDA, logistic regression, and SVM
- Evaluate variable importance using RMSE-based permutation

---

## 📦 Dataset

- **Source**: [Kaggle - Restaurants Revenue Prediction Dataset](https://www.kaggle.com/datasets/mrsimple07/restaurants-revenue-prediction)
- **Type**: Simulated dataset with clean formatting and realistic business features
- **Key Variables**:
  - `Monthly Revenue` (target for regression)
  - `Profit Stat` (scaled revenue)
  - `Success Category` (for classification)
  - Predictors include: number of customers, menu price, marketing spend, cuisine type, reviews, promotions, etc.

---

## 🔍 Key Methods

### 📊 1. **Linear Regression**
- Used to predict continuous revenue
- Achieved an R² of ~0.70
- Model assumptions (normality, equal variance) were reasonably met

### 🔁 2. **Resampling (Cross-validation & Bootstrapping)**
- Used to estimate model performance
- Helped avoid overfitting on small or unbalanced subsets

### 🔢 3. **Classification Techniques**
- **Logistic Regression**
- **Linear Discriminant Analysis (LDA)** – Accuracy: 41.3%
- **Quadratic Discriminant Analysis (QDA)** – Accuracy: 94.6%
- **Support Vector Machine (SVM)** with permutation-based feature importance

### ✅ Success Classification Labels
- **Struggling** (Bottom 25%)
- **Solid** (Mid 50%)
- **Exceeding** (Top 25%)

---

## 📊 Key Findings

- **Most Important Variables**:
  - Number of Customers (strongest predictor)
  - Marketing Spend
  - Menu Price

- QDA outperformed all other classification models by capturing nonlinear relationships in the data.

- SVM permutation testing confirmed the dominance of customer count and marketing spend in predicting success.

---

## 📁 Repository Contents

- `STA_141C_Final_Project.pdf` – Full project report
- `code/` – R scripts for modeling and analysis
- `figures/` – Visualizations: decision boundaries, feature importances, histograms
- `README.md` – This summary file

---

## 🧠 Limitations & Future Work

- Simulated data limits generalizability to real-world restaurant environments
- Profitability might be better modeled with real cost data instead of scaled revenue
- Lack of location or customer demographic data limits explanatory power
- Future work may include ensemble models and real-world datasets

---
