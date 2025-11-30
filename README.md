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
a=input('enter the starting x(n)');
x=input('Enter the x(n) sequence');
n=a:1:length(x)+a-1;
figure(1)
stem(n,x)
xlabel('Time')
ylabel('Amplitude')
title('Input Signal-1')
% INPUT SIGNAL 2
b=input('enter the starting y(n)');
y=input('Enter the y(n) sequence');
m=input('enter the ending y(n)');
n1=b: 1:length(y)+b-1;
figure(2)
stem(n1,y)
xlabel('Time')
ylabel('Amplitude')
title('Input signal-2')
% DISCRETE AUTO CORRELATED SIGNAL
out1=xcorr(x,x)
n2=a-m:1:length(out1)+a-m-1;
figure(3)
stem(n2,out1)
xlabel('Time')
ylabel('Amplitude')
title(' Discrete auto correlated waveform')
% DISCRETE CROSS CORRELATED SIGNAL
Out2=xcorr(x,y);
n3=a-m:1:length(Out2)+a-m-1;
figure(4)
stem(n3,Out2)
xlabel('Time')
ylabel('Amplitude')
title(' Discrete cross correlated waveform')
```

## OUTPUT:
<img width="702" height="629" alt="dsp2(1)" src="https://github.com/user-attachments/assets/eb81016e-26e0-4923-92e1-0eb96f18d5b8" />
<img width="702" height="629" alt="dsp2(2)" src="https://github.com/user-attachments/assets/fd3228cb-e4e5-4413-a13b-b1017def5dca" />
<img width="702" height="629" alt="dsp2(3)" src="https://github.com/user-attachments/assets/637905d8-6191-46a6-99a0-643185afca93" />
<img width="831" height="745" alt="image" src="https://github.com/user-attachments/assets/3189aa5c-9c91-4191-83b5-377e943f4e95" />





## RESULT:
![ds2](https://github.com/user-attachments/assets/68d7f72f-80b3-40f7-9060-4d112ee01729)


