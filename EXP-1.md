# GENERATION OF STANDARD DISCRETE-TIME SIGNALS
# AIM:
To generate and plot standard discrete-time signals using MATLAB.
# APPARATUS REQUIRED:
•	Computer / Laptop
•	MATLAB software
# THEORY:
Discrete-time signals are signals defined only at integer values of time (n).
These signals are basic building blocks in Digital Signal Processing (DSP) and are used for system analysis, filtering, and signal modeling.
Standard discrete-time signals include:
	Unit Impulse
	Unit Step
	Ramp
	Exponential
	Sinusoidal
	Damped Sinusoidal
In MATLAB, discrete-time signals are represented using vectors and plotted using the stem() command.
 Standard Discrete-Time Signals
 
🔹 1. Unit Impulse Signal
δ(n)={■(1,&n=0@0,&n≠0)┤

🔹 2. Unit Step Signal
u(n)={■(1,&n≥0@0,&n<0)┤

🔹 3. Ramp Signal
r(n)=n⋅u(n)

🔹 4. Exponential Signal
x(n)=a^n

🔹 5. Sinusoidal Signal
x(n)=sin⁡(ωn)

🔹 6. Damped Sinusoidal Signal
x(n)=a^n sin⁡(ωn)

# ALGORITHM:
1.	Start the program
2.	Define the sample index n
3.	Generate each standard discrete-time signal
4.	Plot the signal using stem()
5.	Label the axes and title
6.	Stop the program

# MATLAB CODE:
clc;
clear;
close all;

%% Sample index
n = -10:10;

%% 1. Unit Impulse Signal
x1 = (n == 0);
figure;
stem(n, x1, 'filled');
title('Unit Impulse Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 2. Unit Step Signal
x2 = (n >= 0);
figure;
stem(n, x2, 'filled');
title('Unit Step Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 3. Ramp Signal
n1 = 0:10;
x3 = n1;
figure;
stem(n1, x3, 'filled');
title('Ramp Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 4. Exponential Signal
a = 0.8;
x4 = a.^n1;
figure;
stem(n1, x4, 'filled');
title('Exponential Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 5. Sinusoidal Signal
x5 = sin(0.3*pi*n1);
figure;
stem(n1, x5, 'filled');
title('Sinusoidal Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 6. Damped Sinusoidal Signal
x6 = (0.9.^n1).*sin(0.4*pi*n1);
figure;
stem(n1, x6, 'filled');
title('Damped Sinusoidal Signal');
xlabel('n'); ylabel('Amplitude');
grid on;



# OUTPUT GRAPH:
<img width="680" height="551" alt="Screenshot 2026-03-30 195421" src="https://github.com/user-attachments/assets/7403015a-4c93-42a8-9bc0-3f742be92b07" />
<img width="905" height="542" alt="Screenshot 2026-03-31 100644" src="https://github.com/user-attachments/assets/f0667b10-7de0-4d2f-8a23-0ddab0248cae" />
<img width="847" height="550" alt="Screenshot 2026-03-31 100700" src="https://github.com/user-attachments/assets/a7adeafd-1242-4a86-ba37-26aa98ce9946" />
<img width="866" height="562" alt="Screenshot 2026-03-31 100724" src="https://github.com/user-attachments/assets/bdb07b64-2744-48a8-ad6d-86cb257483e7" />
<img width="817" height="550" alt="Screenshot 2026-03-31 100741" src="https://github.com/user-attachments/assets/effccd91-89e3-42d7-b8a1-8e431b7581d9" />
<img width="852" height="546" alt="Screenshot 2026-03-31 100755" src="https://github.com/user-attachments/assets/28e8bad0-cd80-40d9-9242-57393b906604" />

OUTPUT (OBSERVATION)
   Unit impulsee has a single spike at n=0
   Unit step is zero for n<0 and one for n>=0
   Ramp signal increases linearly
   Exponential signal decays since a<1
   Sinusoidal signal oscillates
   Damped sinusoid oscillates
   Damped sinusoid oscillates with decreasing amplitude

# Result :
Thus, standard discrete-time signals were successfully generated and plotted using MATLAB.



