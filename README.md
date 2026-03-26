# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Import the required libraries numpy and scipy.linalg. 
2. Read the coefficient matrix and constant matrix from the user.
3. Use lu_factor() to factorize the coefficient matrix into LU form.
4. Use lu_solve() with the LU factorization and constant matrix to find the solution.
5. Display the solution matrix (X).

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: DEEKSHITHA S
RegisterNumber: 212225100007/25014669
'''
import numpy as np
from scipy.linalg import lu
matrix = eval(input())
P, L, U = lu(matrix) 
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: DEEKSHITHA S
RegisterNumber: 212225100007/25014669
'''

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,piv=lu_factor(A)
X= lu_solve((lu,piv),B)
print(X)
```

## Output:
<img width="1920" height="1080" alt="Screenshot (121)" src="https://github.com/user-attachments/assets/9ac3ed76-23fe-46ca-9e5c-5a7ad80f7408" />

<img width="1920" height="1080" alt="Screenshot (122)" src="https://github.com/user-attachments/assets/a274a6e6-c1a7-46f0-96f5-e72f1422b1ca" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

