# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
step 1:
import the numpy module to use the built-in function for calculation

step 2:
Prepare the list from each linear equation ans assign in np.array()
step 3:
Using the np.linalg.solve(),we can find the solution
step 4:
End the program

## Program:
(i) To find the L and U matrix
```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1" 
import numpy as np
from scipy.linalg import lu_factor,lu_solve
lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)
```

## Output:
<img width="1194" height="458" alt="image" src="https://github.com/user-attachments/assets/ee4f3c29-1901-4707-85bf-07e1c49b3b90" />

<img width="906" height="197" alt="image" src="https://github.com/user-attachments/assets/efe0388b-f270-4beb-816e-436009485dba" />




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

