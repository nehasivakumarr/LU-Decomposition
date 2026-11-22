# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the NumPy and SciPy libraries.
2. Create a matrix using np.array().
3. Using the lu() function, find the permutation matrix (P), lower triangular matrix (L) and upper triangular matrix (U).
4. Display the L and U matrices and find the solution using lu_factor() and lu_solve() functions.

## Program:
(i) To find the L and U matrix
```
'''Program to find the L and U matrix.
Developed by: Neha S
RegisterNumber: 212225100030 '''

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
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
Developed by: Neha S
RegisterNumber: 212225100030
'''
# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(A)
X = lu_solve((lu , piv),b)
print(X)
```

## Output:

<img width="927" height="351" alt="image" src="https://github.com/user-attachments/assets/35def428-d366-4817-856b-d78ea4bee408" />

<img width="682" height="143" alt="image" src="https://github.com/user-attachments/assets/600b0bba-aed8-4d0d-957b-f343c2eb2710" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

