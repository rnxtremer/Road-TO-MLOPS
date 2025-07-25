# 📅 Day 2 — NumPy & Pandas Mastery + Mini Project

## 🎯 Goals for Today
- ✅ Master **NumPy arrays** and operations  
- ✅ Dive deep into **Pandas DataFrames** and transformations  
- ✅ Build a **mini project**: analyze a real dataset (Titanic) from start to finish  

---

## 🛠️ Step 1: Deep Dive into NumPy (1.5 hrs)

### 🧠 Key Concepts
- Array creation, shape, slicing, reshaping  
- Broadcasting, indexing, axis-based operations  
- Mathematical operations: `mean`, `std`, `dot`, matrix ops  

### 📚 Resources
- [NumPy Docs — Quickstart](https://numpy.org/doc/stable/user/quickstart.html)  
- [NumPy 100 Exercises](https://github.com/rougier/numpy-100) *(do 10–15 today)*  
- [Video: NumPy for Data Science](https://www.youtube.com/watch?v=QUT1VHiLmmI)  

---

## 🧠 Step 2: Pandas Mastery (2 hrs)

### Key Concepts
- `read_csv()`, `head()`, `info()`, `describe()`
- Filtering, sorting, selecting, chaining
- `groupby()`, `agg()`, `merge()`, `pivot_table()`
- Handling missing data

### 📚 Resources
- [Pandas DataCamp Tutorial](https://www.datacamp.com/community/tutorials/pandas-tutorial-dataframe-python)
- [Pandas Cheat Sheet PDF](https://pandas.pydata.org/Pandas_Cheat_Sheet.pdf)
- [Video: Pandas in One Hour](https://www.youtube.com/watch?v=zmdjNSmRXF4)

---

##🔨 Step 3: Mini Project — Titanic Dataset EDA (2 hrs)

###📁 Dataset:
Titanic Dataset (Direct CSV Link)

###📘 Task:
Create a notebook that:

Loads the dataset using Pandas

Cleans the data (missing age, drop useless columns)

Performs EDA (use groupby, pivot, etc.)

Visualizes survival rate by class, gender, and age group (matplotlib/seaborn)

Saves the cleaned data as titanic_cleaned.csv

📚 Optional Tools:
matplotlib, seaborn for visualization

import seaborn as sns
sns.barplot(x="Pclass", y="Survived", hue="Sex", data=df)

---

##🧠 Step 4: Git + Reflection (30 min)
Commit your notebook as day2_titanic_eda.ipynb

Push it to your GitHub repo in day2/

Update README with today’s learnings
