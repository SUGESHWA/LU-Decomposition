# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
# 1. Import numpy library.
# 2.Import lu function from scipy library.
# 3.Solve LU decomposition using lu_solve() function.
# 4.print the value.
 

## Program:
(i) To find the L and U matrix
```
#Program to find the L and U matrix.
#Developed by: SUGESHWA S
#RegisterNumber: 212224230277
import numpy as np 
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)

```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: SUGESHWA S
RegisterNumber: 212224230277
'''
import numpy as np
from scipy.linalg import lu, solve

# Define matrix A and vector b
A = np.array([[3, 2, 7],
              [2, 3, 1],
              [3, 4, 1]], dtype=float)

b = np.array([4, 5, 7], dtype=float)

# Perform LU decomposition (with permutation matrix)
P, L, U = lu(A)

# Solve Ly = Pb (forward substitution)
y = np.linalg.solve(L, P @ b)

# Solve Ux = y (backward substitution)
x = np.linalg.solve(U, y)

print(np.round(x, 3))

```

## Output:
# (i)
![Screenshot 2025-05-19 225145](https://github.com/user-attachments/assets/362ec23f-34d2-4a04-9a05-85b40cac9161)
# (ii)
![image](https://github.com/user-attachments/assets/b073a5a3-7609-48c8-91ce-babd9b1b0c00)




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

