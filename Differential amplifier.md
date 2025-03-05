8# Linear integrated circuits 
# Experiment 3

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


Transient analysis 


