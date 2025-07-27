# 📅 Day 3 — Intro to Machine Learning + First ML Pipeline

## 🎯 Goals for Today
- ✅ Understand ML workflow (Supervised Learning)
- ✅ Learn model training, testing, and evaluation
- ✅ Build your first ML pipeline using Scikit-learn
- ✅ Apply it to real data: Classification & Regression

---

## 🔧 Step 1: Core Concepts of ML (1.5 hrs)

### 🧠 Learn These:
- What is Machine Learning?
- Supervised vs Unsupervised Learning
- Classification vs Regression
- Train-Test Split, Overfitting
- Evaluation Metrics: Accuracy, Precision, Recall, F1 Score, ROC

### 📚 Resources:
- [Google ML Crash Course](https://developers.google.com/machine-learning/crash-course)
- [3Blue1Brown: What is a Neural Network](https://www.youtube.com/watch?v=aircAruvnKk)
- [Scikit-learn ML Map](https://scikit-learn.org/stable/tutorial/machine_learning_map/index.html)

---

## ⚙️ Step 2: Scikit-learn Basics (1 hr)

### 🧠 Learn:
- `train_test_split()`, `fit()`, `predict()`
- Models:
  - LogisticRegression
  - DecisionTreeClassifier
  - RandomForestClassifier
  - LinearRegression
- Evaluation Metrics:
  - Accuracy
  - Confusion Matrix
  - Classification Report

### 📚 Docs:
- [Scikit-learn Supervised Models](https://scikit-learn.org/stable/supervised_learning.html)
- [Scikit-learn Cheat Sheet PDF](https://scikit-learn.org/stable/tutorial/machine_learning_map/index.html)

### ✅ Sample Practice:
```python
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LogisticRegression

X = df.drop('Survived', axis=1)
y = df['Survived']
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)

model = LogisticRegression()
model.fit(X_train, y_train)
print("Accuracy:", model.score(X_test, y_test))
```
---
## 🔨 Step 3: Mini ML Project — Titanic Classification (2 hrs)
Use your cleaned Titanic dataset from Day 2.

### 📘 Task:
- Encode categorical columns (Sex, Embarked)

- Handle missing values (if any)

- Normalize numerical columns (optional)

- Train 3 models: Logistic Regression, Decision Tree, Random Forest

- Evaluate using:

     - Accuracy

     - Confusion Matrix

     - Classification Report (precision, recall, F1)

### 📚 Tools:
LabelEncoder, StandardScaler, Pipeline from sklearn

classification_report, confusion_matrix

## ✨ BONUS:
Use GridSearchCV to tune hyperparameters.

## 🌟 Challenge Task: Build a Regression Model
Use this dataset:

[House Prices Dataset (Kaggle)](https://www.kaggle.com/code/prasadperera/the-house-pricing-prediction/data)

Train a Linear Regression model to predict SalePrice.

---
## 📁 Step 4: Organize Your Work (1 hr)
Push both Titanic and HousePrice notebooks to day3/ folder in GitHub repo
