# data-analysis-pandas
import pandas as pd
import numpy as np
df = pd.read_csv("students.csv")
print(df)
df.head()
df.info()
df.describe()
df.shape
df.isnull().sum()
df.duplicated().sum()
high_scorers = df[df["Marks"] > 75]
print(high_scorers)
cs_students = df[df["Department"] == "CSE"]
print(cs_students)
dept_avg = df.groupby("Department")["Marks"].mean()
print(dept_avg)
dept_count = df.groupby("Department")["Student_ID"].count()
print(dept_count)
summary = df.groupby("Department").agg(
    Average_Marks=("Marks", "mean"),
    Max_Marks=("Marks", "max"),
    Min_Marks=("Marks", "min"),
    Student_Count=("Student_ID", "count")
)

print(summary)
