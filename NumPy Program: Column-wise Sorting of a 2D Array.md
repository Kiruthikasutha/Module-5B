# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program
```
import numpy as np
x = np.array([5, 8, 2, 9, 6])
y = np.array([3, 8, 4, 7, 6])
indices = np.where(x >= y)
print("Array x:", x)
print("Array y:", y)
print("Indices where x >= y:", indices[0])

```

## Output
![image](https://github.com/user-attachments/assets/d6bbd098-723c-4753-a592-d9ca11c380fb)

## Result
Thus the program has been successfully executed
# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program
```
import numpy as np

arr = np.array([[12, 5, 7],
                [4, 8, 6],
                [9, 3, 1]])
sorted_arr = np.sort(arr, axis=0)
print("Original Array:\n", arr)
print("Column-wise Sorted Array:\n", sorted_arr)

```
## Output
![image](https://github.com/user-attachments/assets/e6d501c8-acfe-4618-bbb9-d756ee28d857)


## Result
Thus the program has been successfully executed

# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program

```
import numpy as np

arr = np.array([[1, 2, 3],
                [4, 5, 6],
                [7, 8, 9]])

new_col = np.array([10, 11, 12])

arr_modified = np.delete(arr, 1, axis=1)

arr_updated = np.insert(arr_modified, 1, new_col, axis=1)

print("Updated Array:\n", arr_updated)
```
## Output
![image](https://github.com/user-attachments/assets/4fedc72e-e91b-441d-8739-a1aca6a71dac)

## Result
Thus the program has been successfully executed

# Pandas Program: Create and Display a DataFrame with Custom Index Labels

## 🎯 Aim

To create and display a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

---

## 🧠 Algorithm

1. **Import Libraries**: Import the required libraries – `pandas` and `numpy`.
2. **Create Dictionary**: Define a dictionary `exam_data` with keys: `'name'`, `'score'`, `'attempts'`, and `'qualify'`.
3. **Index Labels**: Create a list of custom index labels called `labels`.
4. **Create DataFrame**: Use `pd.DataFrame()` to create the DataFrame by passing the dictionary and index labels.
5. **Display Output**: Display the DataFrame using `print()` or by simply calling the DataFrame variable.

---

## 💻 Program
```
import pandas as pd
import numpy as np

exam_data = {
    'name': ['Anu', 'Bala', 'Chitra', 'David', 'Eva'],
    'score': [85, 92, 76, 88, 90],
    'attempts': [1, 2, 1, 3, 2],
    'qualify': ['yes', 'yes', 'no', 'yes', 'yes']
}

labels = ['a', 'b', 'c', 'd', 'e']

df = pd.DataFrame(exam_data, index=labels)

# Display output
print("Result:\n", df)
```
## Output
![image](https://github.com/user-attachments/assets/846a24f0-a594-4cb5-8785-8ad6b80d2c29)

## Result
Thus the program has been successfully executed

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
    'name': ['Anu', 'Bala'],
    'age': [20, 22],
    'score': [85, 92]
}

student_data2 = {
    'name': ['Chitra', 'David'],
    'age': [23, 21],
    'score': [76, 88]
}

df1 = pd.DataFrame(student_data1)
df2 = pd.DataFrame(student_data2)

df_combined = pd.concat([df1, df2], axis=0, ignore_index=True)

print("Result:\n", df_combined)
```
## Output
![image](https://github.com/user-attachments/assets/87454350-90c1-4a5b-a4cd-b3e97cea8970)

## Result
Thus the program has been successfully executed
