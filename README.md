# SIMULATION-OF-MEAN-AND-VARIANCE-USING-SCILAB-
__AIM:__

To write a program for mean, variance and cross correlation in SCILAB and verify the output. 

__EQUIPMENTS NEEDED:__

.Computer with i3 Processor 

.SCI LAB 

__ALGORITHM:__

1. Define the Function: Specify the function you want to simulate. For example, 
f(x)=sin⁡(x)f(x)=sin(x) or any other function. 
2. Generate Sample Points: Decide on the range and the number of sample points. Generate 
these sample points within the desired range. 
3. Evaluate the Function: Compute the function values at each of these sample points. 
4. Compute Mean, Variance and Cross Correlation: Use Scilab's functions to calculate the 
mean and variance of the computed function values. 
5. Display Results: Output the computed mean variance and Cross Correlation 

__PROCEDURE:__ 

1.Refer Algorithms and write code for the experiment. 

2.Open SCILAB in System 

3.Type your code in New Editor 

4.Save the file 

5.Execute the code If any Error, correct it in code and execute again 
  
6.Verify the generated results

__PROGRAM:__

```
clear;
clc;
clear;
//Mean
function X=f(x)
z =3*(1-x)^2;
X=x*z;
endfunction
a =1;
b =2;
EX=intg(a, b, f);
function Y=c(y)
z =3*(1-y)^2;
Y=y*z;
endfunction
EY=intg(a, b, c);
disp("i) Mean of X = ",EX);
disp("ii)Mean of Y = ",EY);
//variance
function X=g(x),
z=3*(1-x)^2,
X=x^2*z
endfunction
a=2;
b=3;
EX2=intg(a,b,g);
function Y=h(y)
z=3*(1-y)^2,
Y=y^2*z
endfunction
EY2=intg(a,b,h);
vX2=EX2-(EX)^2;
vY2=EY2-(EY)^2;
disp("iii)Variance of X",vX2);
disp("iv) Variance of Y",vY2);

//Cross correlation
x= input("type in the reference sequence=");
y= input("type in the second sequence=");
n1=max(size(y))-1;
n2=max(size(x))-1;
r=corr(x,y,n1);
plot2d3('gnn',r);
```

__OUTPUT GRAPH:__

<img width="501" height="283" alt="image" src="https://github.com/user-attachments/assets/9eae18a1-4aa4-443f-8384-6394370ec0bc" />

<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/cf177e9a-f13b-4c64-ac9e-8ee828fc4cde" />

__RESULT:__

Thus, the mean and variance and cross correlation are executed in SCI-Lab

