# 🧮 List Comprehension:Transpose of Matrix 

## 🎯 AIM:
To write a Python program to compute the **transpose** of a matrix using **list comprehension**.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `r` and `c` to represent the number of rows and columns of the matrix.
3. Get the values of `r` and `c` from the user.
4. Define a function `create(r, c)` to create the matrix by reading the elements from the user.
5. Use **list comprehension** to calculate the transpose of the matrix.
6. Print the transposed matrix.
7. **Stop**

---

## 💻 PROGRAM:
```
def read_matrix(r,c):
    matrix = [[0]*c for row in range(r)]
    for i in range(r):
        lines = list(map(int, input().split()))
        for j in range(c):
            matrix[i][j] = lines[j]
    return matrix
def print_matrix(M):
    print("Matrix:")
    for i in range(len(M)):
        for j in range(len(M[0])):
            print(M[i][j],end=" ")
        print()
def transpose(M):
    result = [[0]*(len(M)) for rows in range(len(M[0]))]
    for i in range(len(M)):
        for j in range(len(M[0])):
            result[j][i] = M[i][j]
    return result

```

## OUTPUT:
<img width="1168" height="476" alt="444527311-234862d9-aaec-4674-9a0d-7438f3e4139f" src="https://github.com/user-attachments/assets/0fe9fafd-9968-41a9-86cb-5074ff2c2491" />

## RESULT:
Thus the ouput is verified.
