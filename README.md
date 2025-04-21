# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. import numpy as np
2. get input from the user
3. calculate the X0, X1 and X2 values by Gaussian elimination.
4. print the values
5. end the program


## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: aravind.p
RegisterNumber: 212224240015

import numpy as np
a=np.array([[1,2,4,18],[2,12,-2,9],[5,26,5,14]])
n=3
for i in range(n):
    for j in range(i+1,n):
        ratio=a[j][i]/a[i][i]
        for k in range(n+1):
            a[j][k] -= ratio * a[i][k]
x=np.zeros(n)
for i in range(n-1,-1,-1):
    x[i] = a[i][n]
    for j in range(i+1,n):
        x[i] -= a[i][j] * x[j]
    x[i] /= a[i][i]
print(" ".join([f"X{i} = {x[i]:.2f}" for i in range(n)]))
*/
```

## Output:
![gaussian elimination]()![Screenshot 2025-04-16 143159](https://github.com/user-attachments/assets/a4d2c80d-3715-4e88-94f0-4adcc8ea8634)



## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

