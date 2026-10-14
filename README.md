# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
```
 (i)5a
 1. import numpy and from scipy.linalg import lu 
 2. get input from  and store it as a matrix by using array from numpy
 3. solve for solution using lu function from scipy.linalg 
 4. print the solution
   
 (ii)5b
 1.import numpy as np and from scipy.linalg import lu_factor,lu_solve
 2.get two input from user and store the two as a matrix using array from numpy
 3.solve for solution using lu_factor and lu_solve function from scipy.linalg 
 4.print the solution
```
## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: M.K.JEEVITH
RegisterNumber: 26018300
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as n
from scipy.linalg import lu
a=n.array(eval(input()))
p,l,u=lu(a)
print(l)
print(u)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: M.K.JEEVITH
RegisterNumber: 26018300
'''

# To print X matrix (solution to the equations)
import os 
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
l,p=lu_factor(a)
x=lu_solve((l,p),b)
print(x)
```

## Output:
(i)
<img width="1468" height="817" alt="Screenshot 2026-10-14 085727" src="https://github.com/user-attachments/assets/438131f1-99fa-4ef5-91c7-2fe824112c81" />
(ii)
<img width="1477" height="622" alt="Screenshot 2026-10-14 085747" src="https://github.com/user-attachments/assets/a5f46e97-f8d8-4b74-bb38-41b72848a41a" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

