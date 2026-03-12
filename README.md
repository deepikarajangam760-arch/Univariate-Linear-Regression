# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Get the independent variable X and dependent variable Y.
2.	Calculate the mean of the X -values and the mean of the Y -values.
3.	Find the slope m of the line of best fit using the formula.
 ![eqn1](./eq1.jpg)
4.	Compute the y -intercept of the line by using the formula:
![eqn2](./eq2.jpg)  
5.	Use the slope m and the y -intercept to form the equation of the line.
6.	Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```

import numpy as np
import matplotlib.pyplot as plt
x=np.array([0,1,2,3,4,5,6,7,8,9])
y=np.array([1,3,2,5,7,8,8,9,10,12])
plt.scatter(x,y)
plt.show()
```
```
xm=np.mean(x)
ym=np.mean(y)

num=0
den=0
for i in range(len(x)):
    num +=(x[i]- xm)*(y[i]-ym)
    den +=(x[i]-xm)**2
m=num/den
c=ym-m*xm
print(m,c)
```
```
xm=np.mean(x)
ym=np.mean(y)

num=0
den=0
for i in range(len(x)):
    num +=(x[i]- xm)*(y[i]-ym)
    den +=(x[i]-xm)**2
m=num/den
c=ym-m*xm
print(m,c)

```
## Output

<img width="1068" height="762" alt="image" src="https://github.com/user-attachments/assets/751da752-d09a-4717-8251-532a45709e98" />

<img width="1449" height="714" alt="image" src="https://github.com/user-attachments/assets/f93a8053-fae8-438d-9865-086c33412c23" />

<img width="1160" height="829" alt="image" src="https://github.com/user-attachments/assets/9560b6bf-89be-4b50-8fb3-49d668073040" />


## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
