# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
## (i) To find the L and U matrix

#### Step 1: Import the required modules numpy and scipy.linalg.lu.
#### Step 2: Read the input matrix and convert it into a NumPy array.
#### Step 3: Apply the lu() function to decompose the matrix into P, L, and U.
#### Step 4: Print the L and U matrices and end the program.

## (ii) To solve a matrix using LU decomposition

#### Step 1: Import the required modules numpy and scipy.linalg.lu_factor, lu_solve.
#### Step 2: Read the coefficient matrix and constant matrix, then convert them into NumPy arrays.
#### Step 3: Use lu_factor() to factorize the matrix and lu_solve() to compute the solution.
#### Step 4: Print the solution vector X and end the program.


## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: JEFFRIN I
RegisterNumber: 212225240060
'''
import numpy as np
from scipy.linalg import lu
matrix = np.array(eval(input()))
P, L, U = lu(matrix)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: JEFFRIN I
RegisterNumber: 212225240060
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
matrix = np.array(eval(input()))
constant = np.array(eval(input()))
piv,lu = lu_factor(matrix)
result = lu_solve((piv,lu),constant)
print(result)
```

## Output:
![alt text](<Screenshot 2026-02-10 201629.png>)

![alt text](<Screenshot 2026-02-10 201702.png>)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

