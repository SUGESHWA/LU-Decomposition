# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import numpy library.
2.Import lu function from scipy library.
3.Solve LU decomposition using lu_solve() function.
4.print the value.
 

## Program:
(i) To find the L and U matrix
```
#Program to find the L and U matrix.
#Developed by: SUGESHWA S
#RegisterNumber: 24900706
import numpy as np 
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)

```
(ii) To find the LU Decomposition of a matrix
```
#Program to find the LU Decomposition of a matrix.
#Developed by: SUGESHWA S
#RegisterNumber: 24900706
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(A)
x = lu_solve((lu,piv),b)
print(x)


```

## Output:
![image](https://github.com/user-attachments/assets/8949415a-90d9-47bd-8bc7-982561e4eb37)



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

