# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
for (i)
1. import numpy and the lu func. from scipy.linalg.
2. use eval(input()) to take the input matrix and convert it into a Numpy array
3. apply the lu() func. to decompose the matrix into permutation(P), lower triangular(L) and upper triangular(U) matrices
4. print the L and U matrices

for (ii)
1. import numpy and the lu_factor and lu_solve func.from the scipy.linalg.
2. use eval(input()) to take the co-efficient matrix A and right-hand side vector (b)
3. apply the lu_factor() func. to factorize the matrix  
4. use the lu_solve() function to solve the linear quations
5. print the source vector(x) 

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: 
RegisterNumber: 
'''
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
RegisterNumber: 24006077

```
(ii) To find the LU Decomposition of a matrix
```
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(A)
x = lu_solve((lu, piv), b)
print(x)

RegisterNumber: 24006077

```

## Output:
![Screenshot 2024-12-02 110236](https://github.com/user-attachments/assets/e6ef14e2-6d91-46dd-8fff-7c457f8a9b45)

![lu decomposition]()

![Screenshot 2024-12-02 110305](https://github.com/user-attachments/assets/aa4ad37e-a67a-4f73-8e11-b17a58b63171)



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

