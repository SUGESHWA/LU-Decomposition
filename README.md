# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

### Algorithm
1.Import necessary libraries: Import numpy as np and lu from scipy.linalg.

2.Get matrix input: Read the matrix A from the user using input() and convert it to a NumPy array with np.array(eval(input())).

3.Perform LU decomposition: Use lu(A) to decompose matrix A into P, L, and U.

4.Extract results: Get the lower triangular matrix L and upper triangular matrix U.

5.Display output: Print matrices L and U using the print() function.
### Algorthim (ii)

1.Import required libraries: Import numpy as np and lu_factor, lu_solve from scipy.linalg.

2.Take input: Read matrix A and vector b from the user using input() and convert them to NumPy arrays.

3.LU factorization: Use lu_factor(A) to compute the LU decomposition and pivot indices of matrix A.

4.Solve the system: Use lu_solve((lu, piv), b) to find the solution vector X for the equation AX = b.

5.Display the result: Print the solution vector X using print().
 

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

