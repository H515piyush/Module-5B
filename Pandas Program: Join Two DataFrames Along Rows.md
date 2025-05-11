# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program
```
import pandas as pd

student_data1 = {
    'name': ['Alice', 'Bob'],
    'score': [85, 90]
}

student_data2 = {
    'name': ['Charlie', 'David'],
    'score': [78, 92]
}

df1 = pd.DataFrame(student_data1)
df2 = pd.DataFrame(student_data2)

combined_df = pd.concat([df1, df2], axis=0)

print(combined_df)
```



## Output
```
      name  score
0    Alice     85
1      Bob     90
0  Charlie     78
1    David     92
```
## Result

The program successfully joins two DataFrames row-wise using pd.concat() and stores the result in a new DataFrame.
