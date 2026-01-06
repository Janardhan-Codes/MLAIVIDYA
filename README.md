<!-- Step 1: Load Dataset

import pandas as pd

df = pd.read_csv("../data/StudentsPerformance.csv")
df.head()

We load the dataset using pandas to inspect its structure. -->


<!-- 
Step 2: Understand the Data

df.shape
df.columns
df.info()
df.describe()


Rows = students

Columns = features

Target = math score -->



<!-- Step 3: Handle Categorical Data

ML models need numbers, not text.

We convert text → numbers using One-Hot Encoding.

df_encoded = pd.get_dummies(df, drop_first=True)
df_encoded.head()


One-Hot Encoding converts categorical columns into numerical format. -->

<!-- Step 4: Split X and y

X = df_encoded.drop("math score", axis=1)
y = df_encoded["math score"] 

-->