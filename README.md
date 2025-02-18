# Linear Integrated Circuit 1

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
Id=50×10^-5/1.8
  =2.77×10^-5 A

![IMG-20250214-WA0002](https://github.com/user-attachments/assets/7ad1571a-69d0-4421-8d78-09ba4aaafc52)

![SAVE_20250217_214721](https://github.com/user-attachments/assets/f41cfddc-4ee7-4b3b-bc79-6a22a6c81a4d)

![SAVE_20250217_215136](https://github.com/user-attachments/assets/266dab14-666d-4ae4-a7f6-3dbb1a42153c)

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

For cmosn:
length=33u
width=30u


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
In the above by calculation came to know that nmos operating in saturation where (Id) drain current controlled by gate Above circuit we can say that Vout taken at drain of nmos.






# Linear Integrated circuit 2

Aim:DC,AC and transient analysis of cs amplifier having both pmos and cmos.

Overview of circuit:
Here Vin=0.9
Vdd=1.8V
In above circuit need to get Vout=1.77V

Introduction:
In circuit 1 considered power by that got current value.Here also should consider same value.So
Id=2.77×10^-5

Circuit design:

![IMG_20250218_111324](https://github.com/user-attachments/assets/fffb21df-51a9-45ec-803f-7637f3511e75)

Here some trial and error values 





| PMOS (L)  | PMOS (W) | NMOS (L)  | NMOS (W) | Current (A)   |
|-----------|---------|-----------|---------|--------------|
| 180 nm    | 33 µm  | 39 µm     | 35 µm   | 2.73887e⁻⁵   |
| 180 nm    | 35 µm  | 39 µm     | 34 µm   | 2.66056e⁻⁵   |
| 180 nm    | 36 µm  | 39 µm     | 33 µm   | 2.58225e⁻⁵   |










DC analysis:
As mentioned above first should consider DC sweep then select dc opt.
Before that by trial and error method try to get near value for Id and Vout.
Above criteria should be considered.

![IMG-20250217-WA0020](https://github.com/user-attachments/assets/e098ef71-dcf7-48d5-8eca-4533c30b470a)



Transient analysis:
We should follow above conditions which are used for circuit 1 in V1.

![IMG-20250217-WA0017](https://github.com/user-attachments/assets/4c2ab16b-5b9d-4832-b613-f10624ffe842)

![IMG-20250217-WA0022](https://github.com/user-attachments/assets/d2d7055e-ece1-43e9-9185-cc24086a4bba)




AC analysis:
For ac analysis should follow same steps.
![IMG-20250217-WA0021](https://github.com/user-attachments/assets/8fd6fe29-590d-4330-a3ab-6ac8f841b6be)


Inference:
Considering above circuit we can say that by This simulation tests a CMOS inverter circuit. A 1.8V power supply (V1) powers the circuit, while a sine wave input (V2) checks its response. A bias voltage (V3 = 0.4V) helps the transistors (M1 = NMOS, M2 = PMOS) switch states. 







