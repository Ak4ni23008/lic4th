# EXP - 6

# CURRENT MIRROR 

## PART A

![image](https://github.com/user-attachments/assets/53515a58-83de-47aa-a7f1-b057e3f370fb)


### **Part A: Current Mirror Design & Analysis**  

1) **Design for Av ≤ -10V/V**  
   - **Given:** Vdd = 1.8V, P ≤ 1mW  
   - **Current Mirror Ratios:** 1:1 and 1:2  
   - Choose W/L to achieve required gain while maintaining power limits.  

2) **DC Analysis**  
   - Determine Vgs, Vds, and bias currents.  
   - Ensure transistors remain in saturation for proper mirroring.  

3) **Current Mirror Analysis with Different L**  
   - **Case 1:** L = 180 nm, (W/L) = x  
   - **Case 2:** L = 500 nm, (W/L) = x  
   - **Case 3:** L = 1 µm, (W/L) = x  
   - Compare impact on mirroring accuracy.  

4) **Transient & AC Analysis**  
   - **Max Output Swing:** Find voltage range before distortion.  
   - **Bandwidth:** Measure frequency response.  

###  DC ANALYSIS 

To achieve the required current based on the given ratio, the chosen W/L values are:

M1: 3µm / 180nm

M2: 3µm / 180nm

M3: 3µm / 180nm

The Vin is set to ensure the transistors remain in the saturation region, so the selected Vin = 0.838V.

for 1:1 ratio, Iref = Ix

So, Iref = It / 2

It = P / Vdd

It = 1mW / 1.8V

It = 0.555mA

Therefore, Iref = 0.2778mA

![image](https://github.com/user-attachments/assets/f1e019b7-bb57-4369-8af1-a6763c055171)

### TRANSIENT ANALYSIS 

### **Steps for Transient Analysis:**  

1. USE **AC signal**.  
2. Use **SINE(0.8, 50mV, 1kHz)** as the signal source.  
3. Go to **"Simulate" > "Edit Simulation Cmd" > "Transient"**.  
4. Set **Stop Time** to **10ms**.  
5. Run the simulation.

![image](https://github.com/user-attachments/assets/866d37e0-301d-4dfe-aec9-094dde9fd5d8)

### AC ANALYSIS 

### **AC Analysis Waveform:**  

1. Open the **Simulation** tab and select **AC Analysis**.  
2. In the **AC Analysis** tab, set **Type of Sweep** to **Decade**.  
3. Enter the **number of points per decade** (e.g., 20).  
4. Set the **frequency range** from **0.1Hz to 1THz**.

![image](https://github.com/user-attachments/assets/9d5704bc-f044-4ef0-8db5-788d08779dcb)

gain in output is 21 but expected is 20db. 3db is 2.85

![image](https://github.com/user-attachments/assets/bffb9181-af6a-4177-ac89-fbee86eb917d)

## FOR RATIO (1:2)







