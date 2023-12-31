# Exp-05-LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm

## (i) To find the L and U matrix
### 1. Import numpy library and import lu from scipy.linalg
### 2. Obtain input and perform LU decomposition
### 3. Print the lower triangular matrix L
### 4. Print the upper triangular matrix U

## (ii) To find the LU Decomposition of a matrix
### 1. Import numpy library and import lu from scipy.linalg
### 2. Obtain input and factorize
### 3. Get right-hand side vector
### 4. Solve the system and print the solution

## Program:
(i) To find the L and U matrix
```
# Program to find L and U matrix using LU decomposition.
# Developed by: P.LOKNAATH
# RegisterNumber: 212223240080

import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
# Program to solve a matrix using LU decomposition.
# Developed by: P.LOKNAATH
# RegisterNumber: 212223240080

# To print X matrix (solution to the equations)

import numpy as np
from scipy.linalg import lu_factor,lu_solve
A = np.array(eval(input()))
B = np.array(eval(input()))
lu,piv = lu_factor(A)
x = lu_solve((lu,piv),B)
print(x)

```

## Output:
![1](https://github.com/AkilaMohan/LU-Decomposition/assets/145742558/7baddcf2-864c-49b3-96e0-c67866ec8c26)

![2](https://github.com/AkilaMohan/LU-Decomposition/assets/145742558/a6fedb7a-6284-4852-8a13-a49f1e62b20f)



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

