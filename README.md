
EXPERIMENT 1

q) in the given below circuit find the DC operating point,gain using transient analysis and AC analysis for different values of RD and W/l ratio .

 ![image](https://github.com/user-attachments/assets/e24d01dd-3817-4812-8027-e1ef4ba223b1)

Aim:To find dc opt point, gain using transient analysis and AC analysis .
Components: resistor, MOSFET, DC power supply.
Procedure:
 Do the circuit connection as shown.
Connect dc power supply to gate and drain terminal and connect source to ground .
Gate voltage supplied is 0.9v and Vdd is 1.8v .

DC analysis 

input voltage is 0.9v connected to gate terminal and VDD is 1.8v.

RD = 1Kohm

ID=55uA

To match id value we need to set the w/l value.



The q point obtained is (1.74v,56uA).

![image](https://github.com/user-attachments/assets/967d9c7d-c88a-48ad-b364-f7132056c87c)


Transient analysis 

analysis used to observe chnages in v and i over time with respect to vin.

input voltage , change it to sine wave with dc offset 0.9v , amplitude 50mv and frequency of 1khz .

![image](https://github.com/user-attachments/assets/5986382a-a277-4c75-9144-914b82291e07)

input and output waveform,

![image](https://github.com/user-attachments/assets/b6d81f1c-3b19-4c33-a119-0613d4613e9b)

Gain=vout/vin

vout=1.79

vin=900mv

Av=2 (approximately)

Ac analysis 

Here we are analysing ckt with different values of frequency.

Select type of sweep to decade , 20 points per decade , start and end frequeny are 0.1 to 1T.

![image](https://github.com/user-attachments/assets/63bafc40-9279-49ba-a236-5c2cd951b9ed)

AC analysis behaviour

![image](https://github.com/user-attachments/assets/25e6f5a1-e877-459c-90ce-ba2cf69ae624)

Graphs

![image](https://github.com/user-attachments/assets/c6f1c7d7-887e-4882-ae6a-6e48442a27b4)

INFERENCE

a)we can vary id by changing aspect ratio.if channel length of the mosfet reduced then short channel effect play imp role.

b)due to phase sift in cs amplifier the output is inverted 



REPLACE RD WITH MOSFET

Length and width of the pmos and nmos are 180nm and 0.2um.

to find vb , vgs<vth , vg-vs<vth

from tsmc lib , vth = -0.3906v

vs=1.8v

vg<1.4094v

vg should be less than 1.4 , assuming vb as 1.25v

circuit diagram

![image](https://github.com/user-attachments/assets/e4791b32-bf8c-477d-9ff2-410734482fdb)

dc opt point

![image](https://github.com/user-attachments/assets/ea57971e-2652-4a8e-b572-19609517371e)

mosfet still working in saturation region.

TRANSIENT ANALYSIS 

dc offset value has 0.9v , amplitude as 50mv and 1k frequency , stop time has 10ms

![WhatsApp Image 2025-02-17 at 22 32 41](https://github.com/user-attachments/assets/28fb2540-4964-4807-9772-0d89909ebf49)

gain=(1.43-1.31/100mv)= 1.2

AC ANALYSIS

![image](https://github.com/user-attachments/assets/bf5ecf59-97ac-443a-84a6-af0b0435da45)

INFERENCE

 CKT 1 resistor gives well balanced gain and bandwidth.CKT 2 high gain low bandwidth.choice of load plays role in finding performance of the 

 ckt components.this visualise how gain, bandwidth changes has ckt changes
























# lic4th
