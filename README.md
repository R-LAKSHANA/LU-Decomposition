# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
(i) To find the L and U matrix.

    1.Import the lu from scipy.linalg to use the built-in functions for calculation.
    2.Get the matrix from the user.
    3.Assign the values of lu() in vaiable as it return 3 values.
    4.Print L and U matrix.

(ii) To find the LU Decomposition of a matrix

    1.Import lu_factor and lu_solve from scipy.linalg.
    2.Get the matrix from the user.
    3.Assign the values of lu_factor() in variable as it returns 2 values.
    4.Apply lu_solve().
    5.Print the LU Decomposition of the matrix.

## Program:
(i) To find the L and U matrix
```python
'''
Program to find the L and U matrix.
Developed by: R LAKSHANA
RegisterNumber: 22004909
'''
import numpy as np
from scipy.linalg import lu
A=eval(input())
P,L,U=lu(A)
print(L)
print(U)
```

(ii) To find the LU Decomposition of a matrix
```python
'''
Program to find the LU Decomposition of a matrix.
Developed by: R LAKSHANA
RegisterNumber: 22004909
'''
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=eval(input())
B=eval(input())
lu,piv=lu_factor(A)
x=lu_solve((lu,piv),B)
print(x)
```

## Output:

(i) Output for L and U matrix.

![l and u matrix](/L_and_U_matrix.png) 

(ii) Output for LU Decomposition of a matrix.

![lu decomposition](/LU_decomposition.png)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

