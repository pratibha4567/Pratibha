# Linear Integrated Circuit experiment:1

Aim:DC,AC and Transient analysis for the given circuit of cs amplifier.

Given information: Vdd=1.8V,power=50uW,Vin=0.9V, 180nm technology.

Introduction:
In the above given information we had power and Vdd.By this we can calculate Id value which is required one.
The given circuit is a CS amplifier.
Input Signal (Vin): Applied to the gate terminal of the FET.
Drain Resistor (Rd): Connected to the drain terminal to develop the amplified output.

Circuit design:

![1000140280](https://github.com/user-attachments/assets/39bc3cc1-c035-4277-9d42-45091b7362d1)

DC analysis:
In the above circuit we know power and voltage by this calculate current 
given power=50uW,Vdd=1.8V
Id=50×10^-6/1.8
  =2.77×10^-5 A

![IMG-20250214-WA0002](https://github.com/user-attachments/assets/7ad1571a-69d0-4421-8d78-09ba4aaafc52)


By doing trial and error method got allmost near value.
For dc analysis first consider DC sweep in that we need to fill information.Example for the given circuit.
Above should be in saturation.
Vds>Vov.
Vds=Vout=1.77V
Vov=Vgs-Vt
   =0.9-0.366
Vov=0.534V
Vds>Vov
So it's in saturation.

Name 1st source to sweep:V2
Type of sweep: linear.
Start value:0
Stop value:1.8
Increment: 0.1
then should select dc opt to obtain above analysis 
![IMG-20250214-WA0013(1)](https://github.com/user-attachments/assets/69f0959f-28a5-4c2a-a0b3-3e3985c6cab1)



Transient analysis:

It can be done by considering.
Stop time:1m
then put value for V1
select sine wave,
dc offset:0.9
amplitude:50m
frequency:1k
![IMG-20250214-WA0006](https://github.com/user-attachments/assets/b139588f-33a9-4eea-9b5f-0300a6cd5c78)

![IMG-20250214-WA0008](https://github.com/user-attachments/assets/ad9af4ad-b4a1-4085-adfd-9c737dd77070)




AC analysis:
For ac analysis 
Type of sweep:decade.
No. of points per decade:20
start frequency:1k
stop frequency:1T

then should select ac amplitude:50m

![IMG-20250214-WA0009](https://github.com/user-attachments/assets/513c350b-5610-4833-8027-e8f8896eb83c)

Inference:
From above we can say that 






Linear Integrated circuit experiment 2

Aim:DC,AC and transient analysis of cs amplifier having both pmos and cmos.

Overview of circuit:


