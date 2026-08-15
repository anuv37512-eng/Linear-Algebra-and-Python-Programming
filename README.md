Part 2: Python Implementation

**1. Basic Data Structures**
The function should count how many times each integer occurs in a list.

**CODE**
def count_frequencies(data_list):
    frequency = {}

    for number in data_list:
        if number in frequency:
            frequency[number] += 1
        else:
            frequency[number] = 1

    return frequency


# Example
data = [1, 2, 2, 3, 3, 3, 4, 4]

result = count_frequencies(data)

print(result)

**OUTPUT**
{1: 1, 2: 2, 3: 3, 4: 2}

**2. NumPy Array Operations**
We recreate matrices A and B and calculate their dot product.

**CODE**
import numpy as np

# Define matrix A
A = np.array([
    [1, 2],
    [3, 4]
])

# Define matrix B
B = np.array([
    [5, 6],
    [7, 8]
])

# Calculate the dot product
result = np.dot(A, B)

# Display the result
print("Matrix A:")
print(A)

print("\nMatrix B:")
print(B)

print("\nA * B:")
print(result)

**OUTOUT**
Matrix A:
[[1 2]
 [3 4]]

Matrix B:
[[5 6]
 [7 8]]

A * B:
[[19 22]
 [43 50]]

 **3. Data Processing — Pearson Correlation**
This program reads a CSV file containing two numerical columns and calculates their Pearson correlation coefficient.

Example CSV file: data.csv
Column1,Column2
10,20
20,40
30,60
40,80
50,100

**CODE**
import pandas as pd

# Read the CSV file
data = pd.read_csv("data.csv")

# Calculate Pearson correlation
correlation = data["Column1"].corr(data["Column2"])

# Display the result
print("Pearson Correlation Coefficient:", correlation)

**OUTPUT**
Pearson Correlation Coefficient: 1.0
A correlation coefficient of 1.0 means there is a perfect positive linear relationship between the two columns.

**FINAL ANSWER**
| Question           | Answer                                                              |
| ------------------ | ------------------------------------------------------------------- |
| Matrix (AB)        | (\begin{bmatrix}19&22\43&50\end{bmatrix})                           |
| Determinant of (A) | (-2)                                                                |
| Inverse of (A)     | (\begin{bmatrix}-2&1\1.5&-0.5\end{bmatrix})                         |
| Linear equations   | (x=1,\ y=3)                                                         |
| Eigenvector        | Non-zero vector whose direction remains unchanged by transformation |
| Eigenvalue         | Scalar factor by which the eigenvector is scaled                    |



