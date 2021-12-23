# LU Decomposition without zero on the diagonal

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### 1. To Find L and U matrices with LU Decomposition
Step 1: Get the matrix from the user.

Step 2: Using "from scipy.linalg import lu" to import scipy (LU) module.

Step 3: Using "L,U=lu(a)" we can get the matrix of L and U.

Step 4: Print the result matrices (L and U Matrices).

Step 5: End of the Program.


### 2. To Find X matrix with LU Decomposition
Step 1: Get the matrix from the user.

Step 2: Using "from scipy.linalg import lu_factor,lu_solve" to import scipy module for factorization and solving X.

Step 3: Using "lu,piv=lu_factor(a)" 

Step 4: 

Step 5: End of the Program.


## Program:
```
'''Program to find L and U matrix using LU decomposition.
Developed by: S.ABHISHEK    
RegisterNumber: 21004552
'''

# To print L and U matrix
import numpy as np
from scipy.linalg import lu

a=np.array(eval(input()))
P,L,U=lu(a)
print(L)
print(U)

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve

a=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(a)
x=lu_solve((lu,piv),b)
print(x)
```

## Output:
### 1. To Find L and U matrices with LU Decomposition
![Github Logo](lu_1.png)

### 2. To Find X matrix with LU Decomposition
![Github Logo](lu_2.png)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

