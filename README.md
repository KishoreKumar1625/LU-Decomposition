# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm

### 5A

### Step1: 
Import the required numpy and scipy
### Step2: 
Bring lu from scipy.linalg to handle the actual matrix decomposition
### Step3:
Call the lu(A) function.This splits the target matrix into three seperate output matrices P,L AND U
### Step4:
End the program

### 5B

### Step1:
Import numpy for multi-dimensional array operations
### Step2:
Bring lu from scipy.linalg to handle the actual matrix decomposition
### Step3:
Pass the factorized components (lu, p) along with the right-hand-side matrix to the lu_solve() function to compute the solution matrix x.
### Step4:
End the program



## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.

Developed by: Kishore Kumar P

RegisterNumber: 26002452

'''

import os

os.environ["OPENBLAS_NUM_THREADS"]="1"

import numpy as np

from scipy.linalg import lu

A=np.array(eval(input()),dtype=float)

P,L,U=lu(A)

print(L)

print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.

Developed by: Kishore Kumar P

RegisterNumber: 26002452

'''

# To print X matrix (solution to the equations)

import os

os.environ["OPENBLAS_NUM_THREADS"]="1"

import numpy as np

from scipy.linalg import lu_factor,lu_solve

a=eval(input())

b=eval(input())

l,p=lu_factor(a)

x=lu_solve((l,p),b)

print(x)

```

## Output:
![lu decomposition]()
### 5A INPUT
<img width="1453" height="890" alt="Screenshot 2026-10-14 090939" src="https://github.com/user-attachments/assets/d0ef506a-2415-4ba1-a697-f9a3eb11863e" />

### 5A OUTPUT
<img width="1439" height="555" alt="Screenshot 2026-10-14 090956" src="https://github.com/user-attachments/assets/f4c9e7ab-d901-4610-a5b8-49dce55d4dc4" />

### 5B INPUT
<img width="1269" height="862" alt="Screenshot 2026-10-14 091013" src="https://github.com/user-attachments/assets/291f0482-43b6-4f6b-8442-a3db9ec49013" />

### 5B OUTPUT
<img width="1411" height="256" alt="Screenshot 2026-10-14 091025" src="https://github.com/user-attachments/assets/f4e5a544-f8ea-4ba0-80bd-3102b63c6c3b" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

