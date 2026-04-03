# Digital-Signal-Processing--Correlation
## AIM:
To generate discrete auto correlation and cross correlation of signals using MATLAB.
## APPARATUS REQUIRED:
MATLAB R2012.
## ALGORITHM:
Step 1: Open matlab. Write the program.

Step 2: Read the input sequence 1 and input sequence 2 sequence.

Step 3: Perform auto correlation and cross correlation for both the sequences. 

Step 4: Plot the output sequence with x-label and y-label with suitable title.

Step 5: Terminate the program.


## PROGRAM: 
```
clc; % clear screen
clear all; % clear screen
close all; % close all figure windows

% INPUT SIGNAL-1
a=-3;
x=[2.3,3.4,-4.5,5,6.2,3.9];
n=a:1:length(x)+a-1;

figure(1)
stem(n,x)
xlabel('Time')
ylabel('Amplitude')
title('Input Signal-1')

% INPUT SIGNAL 2
b=-1;
y=[1.5,2.4,3.6,4,-1.8,4.5,5.2];
m=4;
n1=b:1:length(y)+b-1;

figure(2)
stem(n1,y)
xlabel('Time')
ylabel('Amplitude')
title('Input signal-2')

% DISCRETE AUTO CORRELATED SIGNAL
out1=xcorr(x,x);
n2=a-m:1:length(out1)+a-m-1;

figure(3)
stem(n2,out1)
xlabel('Time')
ylabel('Amplitude')
title('Discrete auto correlated waveform')

% DISCRETE CROSS CORRELATED SIGNAL
out2=xcorr(x,y);
n3=a-m:1:length(out2)+a-m-1;

figure(4)
stem(n3,out2)
xlabel('Time')
ylabel('Amplitude')
title('Discrete cross correlated waveform')
```

## OUTPUT:
<img width="1919" height="949" alt="image" src="https://github.com/user-attachments/assets/969f95ea-f7bd-4eb2-867d-ba35a3825c81" />


## RESULT:
<img width="1280" height="960" alt="image" src="https://github.com/user-attachments/assets/4976fce0-2da6-4feb-ab6c-a8130d483b38" />


