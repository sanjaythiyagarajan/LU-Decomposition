# LU Decomposition 

## AIM:

To write a program to find the LU Decomposition of a matrix.

## Equipments Required:

1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Import numpy library using import statement

2.From scipy package import lu_factor() and lu_solve().

3.Get two inputs from user and pass it as matrix array.

4.Find lu and pivot value of first marix using lu_factor().

5.Find solution of the matrix by using lu_solve() by passing lu, pivot values as first argument and second matrix as second argument.

6.Print the solution


## Program:
(i) To find the L and U matrix
```
'''
Program to find L and U matrix using LU decomposition.
Developed by: SANJAY T
RegisterNumber: 212222110039
'''
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
(ii) To find the LU Decomposition of a matrix
```
```
'''Program to solve a matrix using LU decomposition.
Developed by: SANJAY T 
RegisterNumber: 212222110039
'''
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
arr=np.array([[3, 2, 7], [2, 3, 1], [3, 4, 1]])
B=np.array([4, 5, 7])
lu,p=lu_factor(arr)
res=lu_solve((lu,p),B)
print(res)
```

## Output:

![lu decomposition]()
![5a maths](https://github.com/sanjaythiyagarajan/LU-Decomposition/assets/119409242/293db437-ffe4-4352-8c13-bd243c7facc3)

![5b maths](https://github.com/sanjaythiyagarajan/LU-Decomposition/assets/119409242/f849cbc5-1490-483f-a8e0-ecb7f4fb8cfc)

## Result:

Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

