📅 Day 2 — NumPy, Pandas Mastery + Mini Project
🎯 Goals for Today
Master NumPy arrays and operations

Dive deep into Pandas DataFrames and transformations

Build a mini project: analyze a real dataset from start to finish

🛠️ Step 1: Deep Dive into NumPy (1.5 hrs)
🧠 Key Concepts
Array creation, shape, slicing, reshaping

Broadcasting, indexing, axis-based operations

Math: mean, std, dot product, matrix ops

📚 Resources
NumPy Docs — Quickstart

NumPy 100 Exercises (do 10–15 today)

Video: NumPy for Data Science

✅ Practice
python
Copy
Edit
import numpy as np

a = np.arange(15).reshape(3,5)
print("Shape:", a.shape)
print("Sum along columns:", a.sum(axis=0))
📊 Step 2: Pandas Mastery (2 hrs)
🧠 Key Concepts
read_csv(), head(), info(), describe()

Filtering, sorting, selecting, chaining

groupby(), agg(), merge(), pivot_table()

Handling missing data

📚 Resources
Pandas DataCamp Tutorial

Pandas Cheat Sheet PDF

Video: Pandas in One Hour

✅ Practice
python
Copy
Edit
import pandas as pd

df = pd.read_csv("https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv")
print(df['Age'].mean())
print(df.groupby('Sex')['Survived'].mean())
🔨 Step 3: Mini Project — Titanic Dataset EDA (2 hrs)
📁 Dataset:
Titanic Dataset (Direct CSV Link)

📘 Task:
Create a notebook that:

Loads the dataset using Pandas

Cleans the data (missing age, drop useless columns)

Performs EDA (use groupby, pivot, etc.)

Visualizes survival rate by class, gender, and age group (matplotlib/seaborn)

Saves the cleaned data as titanic_cleaned.csv

📚 Optional Tools:
matplotlib, seaborn for visualization

python
Copy
Edit
import seaborn as sns
sns.barplot(x="Pclass", y="Survived", hue="Sex", data=df)
🧠 Step 4: Git + Reflection (30 min)
Commit your notebook as day2_titanic_eda.ipynb

Push it to your GitHub repo in day2/

Update README with today’s learnings
