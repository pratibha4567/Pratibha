# Linear integrated circuits 
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

3.Double-Ended Input, Single-Ended Output

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


Given that,
P<=3mW
Iss=P/Vdd=1.2mA
Id1=Id2=Iss/2=0.6mA
Rd=Vdd-Vocm/Id1=1.833k ohm
Rss=Vp/Iss=416.66ohm
![IMG-20250310-WA0007](https://github.com/user-attachments/assets/08892298-9ee9-482f-b77c-7daec3264bfc)

Step 1: DC analysis 

DC Analysis in LTSpice is used to find the voltage and current at different points in a circuit when a DC power supply is applied.

It shows the steady values without any time changes.

Use it to check if your circuit is working properly before testing other signals.
![IMG-20250310-WA0025](https://github.com/user-attachments/assets/fdf85428-8412-4006-b007-6261bf023ef8)

![IMG-20250310-WA0029](https://github.com/user-attachments/assets/65349acf-4cea-45b2-978a-691ff759c2d7)

![IMG-20250310-WA0039](https://github.com/user-attachments/assets/3328becd-2538-43d4-8e51-2d18b66db2b7)

Transient analysis:
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
![IMG-20250310-WA0024](https://github.com/user-attachments/assets/888d1179-cfc1-4176-8f13-f46f46eb487a)

![IMG-20250310-WA0016](https://github.com/user-attachments/assets/82a9e9d5-1f9c-43ae-9b3f-50c12fb3dc23)

Output signal 

![IMG-20250310-WA0014](https://github.com/user-attachments/assets/db791fb4-26b9-4f5e-9f97-049375c181c3)

![IMG-20250310-WA0021](https://github.com/user-attachments/assets/94da2b29-8641-4585-8811-e33a6d88c658)

Combination of both input and output signal:
![IMG-20250310-WA0034](https://github.com/user-attachments/assets/d8315050-553c-491f-a7de-5e70d1180f8e)


AC analysis:
Transient Analysis in LTSpice shows how voltages and currents change over time in a circuit when signals like AC or pulse are applied.

It helps to see how the circuit behaves from start to end.

Used for testing circuits with time-varying signals.

For ac analysis 
Type of sweep:decade. 
No. of points per decade:20 
start frequency:0.1
stop frequency:1T
![IMG-20250310-WA0042](https://github.com/user-attachments/assets/52ebfd09-53f9-4bef-bcf7-b69243ded945)
From the plot:

The maximum gain appears to be around 13.5 dB.

The -3 dB point would be at 10.5 dB.


Observing the graph:

The lower cutoff frequency appears to be near 100 MHz.

The upper cutoff frequency is around 1.75 GHz.


Bandwidth Calculation:

\text{Bandwidth} = \text{Upper cutoff frequency} - \text{Lower cutoff frequency}

= 1.75 \text{ GHz} - 100 \text{ MHz} ]

= 1.65 \text{ GHz}

Final Answer:

Bandwidth ≈ 1.65 GHz
![IMG-20250310-WA0054](https://github.com/user-attachments/assets/a06d34a6-a86d-42ad-bc96-1319181009a9)

DC sweep:
Vicm(min)=Vth+Vp=0.495+0.5=0.995V
Vicm(max)=Vdd-Id1(Rd)+Vth=
2.5-1.8(0.6)+0.495=1.915V
Average=1.455V

![IMG-20250310-WA0013](https://github.com/user-attachments/assets/7850ea02-ee24-43f2-a1e0-50049a6ae5bd)



# Circuit 2:

Here we are replacing resistor by current source.

![IMG-20250310-WA0057](https://github.com/user-attachments/assets/f4f6d3a7-e175-4f3e-9a6a-c6cbdca94313)


![IMG-20250310-WA0009](https://github.com/user-attachments/assets/63a7c5b4-5c0a-4613-bb37-9153d6b16089)


DC analysis:
![IMG-20250310-WA0058](https://github.com/user-attachments/assets/e70d4405-f639-4ad2-bea4-8219fb9ec628)

![IMG-20250310-WA0020](https://github.com/user-attachments/assets/3c232765-cf66-4672-b097-a3985f81d8a3)




Transient analysis:

Gain=Vopp/Vipp=0.474/0.1004=4.721

Input waveform:
![IMG-20250310-WA0026](https://github.com/user-attachments/assets/11583536-cbd8-46fa-8e47-dae5961f9cb7)

![IMG-20250310-WA0011](https://github.com/user-attachments/assets/c93657d4-a459-4ba4-9b62-2004db8ee340)

Output waveform:
![IMG-20250310-WA0040](https://github.com/user-attachments/assets/7edb2b36-213b-4108-ac3f-b423e2e500e8)

![IMG-20250310-WA0008](https://github.com/user-attachments/assets/2927f3a3-c935-4a92-8f6b-b212a0e0eb71)

Combination of input and output waveform:
![IMG-20250310-WA0012](https://github.com/user-attachments/assets/713d9f33-aac6-4469-bb22-3558870b839b)




AC analysis:

![IMG-20250310-WA0048(1)](https://github.com/user-attachments/assets/61d88597-29a0-499a-b33f-0759e9674f33)

Bandwidth for above plot:
At 1.220 GHz, the gain is 13.620 dB.

The -3 dB point (relative to the peak gain) should be around 10.62 dB.

The lower cutoff frequency is still approximately 100 MHz.

The upper cutoff frequency now appears to be around 1.22 GHz.


Bandwidth Calculation:

\text{Bandwidth} = \text{Upper cutoff frequency} - \text{Lower cutoff frequency}

= 1.22 \text{ GHz} - 100 \text{ MHz} ]

= 1.12 \text{ GHz}

Final Answer:

Bandwidth ≈ 1.12 GHz
![IMG-20250310-WA0049](https://github.com/user-attachments/assets/faf3f222-3a57-4264-afe7-7b2cc30f62fc)



DC sweep:

![IMG-20250305-WA0060](https://github.com/user-attachments/assets/7f502082-7b0d-4de6-8d75-020ae757c95e)


# Circuit 3:
Again we are replacing current source by nmos.
Here we supply voltage for nmos 
Vb=Vth+Vp
Vb =0.495+0.5=0.995V

![IMG-20250310-WA0046](https://github.com/user-attachments/assets/a3f161c1-2e7f-4cf2-912b-05258a256ae4)

DC analysis:

We need to adjust dc operating points by adjusting nmos values.




Transient analysis:
Gain=0.4665/0.09913=4.705

![IMG-20250305-WA0080](https://github.com/user-attachments/assets/086be759-74ff-41c4-81b0-0b2938a0d348)

![IMG-20250305-WA0072](https://github.com/user-attachments/assets/cb8fc3fe-737a-4596-9801-1a585f52e726)

AC analysis:

![IMG-20250305-WA0082](https://github.com/user-attachments/assets/df264fd3-5229-44b7-be59-8c4a42be4cf5)


DC Sweep:

![IMG-20250305-WA0078](https://github.com/user-attachments/assets/0b27f97b-16e7-4004-910f-965cff72ddfd)

Inference:
The differential amplifier circuit is simulated successfully using LTSpice. It amplifies the difference between two input signals while rejecting common signals (noise). The output shows proper amplification with good accuracy. The circuit works linearly within the input range, proving its functionality.


