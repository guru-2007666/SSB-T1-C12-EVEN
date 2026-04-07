# SSB-T1-C12-EVEN
AIM:

To write a program for mean, variance and cross correlation in SCILAB and verify the output.

EQUIPMENTS NEEDED:

.Computer with i3 Processor

.SCI LAB

ALGORITHM:

Define the Function: Specify the function you want to simulate. For example, f(x)=sin⁡(x)f(x)=sin(x) or any other function.
Generate Sample Points: Decide on the range and the number of sample points. Generate these sample points within the desired range.
Evaluate the Function: Compute the function values at each of these sample points.
Compute Mean, Variance and Cross Correlation: Use Scilab's functions to calculate the mean and variance of the computed function values.
Display Results: Output the computed mean variance and Cross Correlation
PROCEDURE:

1.Refer Algorithms and write code for the experiment.

2.Open SCILAB in System

3.Type your code in New Editor

4.Save the file

5.Execute the code If any Error, correct it in code and execute again

6.Verify the generated results

PROGRAM:
```
Am=7.3;
fm=286;
Ac=14.6;
fc=2860;
fs=28600;
t=0:1/fs:2/fm;
m1=Am*cos(2*3.14*fm*t);
subplot(4,1,1);
plot(t, m1);
cl=Ac*cos(2*3.14*fc*t);
subplot(4,1,2);
plot(t,cl);
m2=Am*cos(1.57-(2*3.14*fm*t));
c2=Ac*cos(1.57-(2*3.14*fc*t));
a = cl.*m1;
b = c2.* m2;
c = a + b;
subplot(4,1,3);
plot(t, c);
d=a-b;
subplot(4,1,4);
plot(t, d);

```
OUTPUT GRAPH:

<img width="1919" height="1113" alt="image" src="https://github.com/user-attachments/assets/4584f3c4-f4d0-4453-aba9-7e83c5e1e95f" />


RESULT:

A single sideband suppress carrier is generated using scilab
