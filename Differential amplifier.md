8# Linear integrated circuits 
# Experiment 3
# Circuit 1:

Introduction:
A Differential Amplifier is an electronic circuit that takes two input signals and gives an output.

The key concept of using differential amplifier is to reduce noise signal in audio systems, sensors, and communication circuits.
There are mainly 4 types of Differential Amplifiers based on their input and output configuration:

1. Single-Ended Input, Single-Ended Output

One input signal is applied, and the other input is grounded.

Output is measured at one terminal.

Simple design, but less noise rejection.


2. Single-Ended Input, Double-Ended Output

One input signal is applied, and the other input is grounded.

Output is measured between two output terminals.

Better noise rejection compared to type 1.


3. Double-Ended Input, Single-Ended Output

Two input signals are applied.

Output is measured at one terminal.

Commonly used in operational amplifiers.


4. Double-Ended Input, Double-Ended Output

Two input signals are applied.

Output is measured between two output terminals.

Best noise rejection and accuracy.


The Double-Ended Input, Double-Ended Output type is the most commonly used in advanced applications like sensors and audio systems.

Aim: design differential amplifier for the following
specification.Vdd=2.5V,P<=3mW
Vicm=1.3V,Vocm=1.4V,Vp=0.5V. Perform DC analysis transient analysis and frequency response and extract the required parameters.
![IMG-20250305-WA0028](https://github.com/user-attachments/assets/126d57e8-cc15-4ad5-a98d-6e41236dd6c3)

Given that,
P<=3mW
Iss=P/Vdd=1.2mA
Id1=Id2=Iss/2=0.6mA
Rd=Vdd-Vocm/Id1=1.833k ohm
Rss=Vp/Iss=416.66ohm

Step 1: DC analysis 
![IMG-20250305-WA0025](https://github.com/user-attachments/assets/8ad4c2e5-6c28-44e7-beaf-80ab53a6bec5)


DC Analysis in LTSpice is used to find the voltage and current at different points in a circuit when a DC power supply is applied.

It shows the steady values without any time changes.

Use it to check if your circuit is working properly before testing other signals.
![IMG-20250305-WA0032](https://github.com/user-attachments/assets/a81a8691-ddaf-41ff-8f70-24bd99aaed3c)


Transient analysis 
It can be done by considering.

Stop time:5m

then put value for V1 select sine wave,

dc offset:1.3V

amplitude:50m

frequency:1k
Gain:
Vopp=0.4696V
Vipp=0.1009V
Av=4.654

Input signal:
![IMG-20250305-WA0031](https://github.com/user-attachments/assets/8b14499b-9128-4ce1-b3da-01d35888b704)

Output signal 
![IMG-20250305-WA0033](https://github.com/user-attachments/assets/0efe013d-0b53-49db-ab35-9e67fe20cc1d)

![IMG-20250305-WA0036](https://github.com/user-attachments/assets/43a4bc19-6785-4a51-9b1b-de6b580aab6f)


AC analysis:
Transient Analysis in LTSpice shows how voltages and currents change over time in a circuit when signals like AC or pulse are applied.

It helps to see how the circuit behaves from start to end.

Used for testing circuits with time-varying signals.

For ac analysis 
Type of sweep:decade. 
No. of points per decade:20 
start frequency:0.1
stop frequency:1T

![SAVE_20250306_242731](https://github.com/user-attachments/assets/6358e9f6-326e-4c4b-86f9-5f542f33aec6)

![IMG-20250305-WA0016](https://github.com/user-attachments/assets/2b7daa8c-7a3c-4ee5-953e-5f2f426523d8)

DC sweep:
Vicm(min)=Vth+Vp=0.495+0.5=0.995V
Vicm(max)=Vdd-Id1(Rd)+Vth=
2.5-1.8(0.6)+0.495=1.915V
Average=1.455V

![Screenshot 2025-03-05 222348](https://github.com/user-attachments/assets/cae05e41-f13e-4e3f-bb6d-ac8eb11718df)

![IMG-20250305-WA0063](https://github.com/user-attachments/assets/680e9e87-3eca-4ad6-9de6-101d7688eb6e)


# Circuit 2:

Here we are replacing resistor by current source.

![IMG_20250306_010929](https://github.com/user-attachments/assets/b8ff382b-7db4-4c72-ac42-0bd39a766371)

DC analysis:

![SAVE_20250306_242703](https://github.com/user-attachments/assets/b2b9864e-b2f7-413a-b572-f41b61826b72)


Transient analysis:

Gain=Vopp/Vipp=0.474/0.1004=4.721

![SAVE_20250306_242725](https://github.com/user-attachments/assets/68009fbc-1cd5-4b4e-9f62-268d6c2d9435)

AC analysis:

![IMG-20250305-WA0059](https://github.com/user-attachments/assets/cdbe6c41-ff1e-4ebd-9285-930de0916d8b)

![Screenshot 2025-03-05 222348](https://github.com/user-attachments/assets/84338683-427c-460a-bb2b-b2fb3fab409e)



DC sweep:

![IMG-20250305-WA0060](https://github.com/user-attachments/assets/7f502082-7b0d-4de6-8d75-020ae757c95e)


# Circuit 3:
Again we are replacing current source by nmos.
Here we supply voltage for nmos 
Vb=Vth+Vp
Vb =0.495+0.5=0.995V

DC analysis:

We need to adjust dc operating points by adjusting nmos values.

![IMG-20250305-WA0081](https://github.com/user-attachments/assets/9285db82-f9fd-415e-9de7-8776b2b523a3)

![IMG-20250305-WA0076](https://github.com/user-attachments/assets/d8926182-7802-4083-9a63-f5dcc8f1735e)

Transient analysis:
Gain=0.4665/0.09913=4.705

![IMG-20250305-WA0080](https://github.com/user-attachments/assets/086be759-74ff-41c4-81b0-0b2938a0d348)

![IMG-20250305-WA0072](https://github.com/user-attachments/assets/cb8fc3fe-737a-4596-9801-1a585f52e726)

AC analysis:

![IMG-20250305-WA0082](https://github.com/user-attachments/assets/df264fd3-5229-44b7-be59-8c4a42be4cf5)


DC Sweep:

![IMG-20250305-WA0078](https://github.com/user-attachments/assets/0b27f97b-16e7-4004-910f-965cff72ddfd)

Inference:


