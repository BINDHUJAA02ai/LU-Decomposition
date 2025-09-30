# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Take matrix input from the user and convert it to a NumPy array.

2.Apply LU decomposition using scipy.linalg.lu() to get P, L, and U.

3.Extract the L (lower) and U (upper) triangular matrices.

4.Print the L and U matrices

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by:BINDHUJAA S
RegisterNumber: 212224230038
*/
import numpy as np
from scipy.linalg import lu

A=np.array(eval(input()))
P,L, U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: BINDHUJAA S
RegisterNumber: 212224230038
*/
import numpy as np
from scipy.linalg import lu
A=np.array([[3,2,7],[2,3,1],[3,4,1]])
b=np.array([4,5,7])
P,L,U=lu(A)
y=np.linalg.solve(L, np.dot(P,b))
x=np.linalg.solve(U,y)
print(x)
```

## Output:
![lu decomposition]()
<img width="1408" height="959" alt="Screenshot 2025-09-30 134454" src="https://github.com/user-attachments/assets/897f6759-08f2-42f4-86c2-ab3f9e91ceff" />
<img width="1440" height="952" alt="Screenshot 2025-09-30 134511" src="https://github.com/user-attachments/assets/4f99a525-68d4-472f-bd73-29a58f8aaa15" />




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

