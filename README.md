# LU Decomposition 

~~~
Name: Bala Surya S
Register No: 212225100003
~~~

## AIM:

To write a program to find the LU Decomposition of a matrix.

## Equipments Required:

1. Hardware – PCs
  
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm

1.Start the program

2.Import the necessary libraries(numpy,scipy.linalg)

3.Define the matrix using numpy

4.Use lu(),lu_solve(),lu_factor() to get the solutions

5.End the program

## Program:

(i) Use LU Decomposition to find L and U matrix.

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

(ii) Use LU Decomposition to solve a matrix.

```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)
```

## Output:

<img width="1175" height="444" alt="1" src="https://github.com/user-attachments/assets/fa20f81e-1b85-46d1-b08f-ed88c6f2aa74" />


<img width="869" height="184" alt="2" src="https://github.com/user-attachments/assets/3834534d-c1e3-4d82-9147-0b14baca1ab0" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

