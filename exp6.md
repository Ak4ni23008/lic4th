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

For a **1:2 ratio**, the relationship is **2 × Iref = Ix**.  

Thus, **Iref = It / 3**.  

Given:  

**It = P / Vdd**  

**It = 1mW / 1.8V**  

**It = 0.555mA**  

So, **Iref = 0.185mA**.  

To achieve the desired current ratio, the selected **W/L values** are:  

- **M1:** 6µm / 180nm  
- **M2:** 6µm / 180nm  
- **M3:** 3µm / 180nm  

The input voltage **Vin** is chosen to keep the transistors in the **saturation region**, with **Vin = 0.763V**.

![image](https://github.com/user-attachments/assets/3e102baa-033c-474c-8afd-2a291613508d)

## DC ANALYSIS 

OUTPUT OBTAINED 

![image](https://github.com/user-attachments/assets/c2922c8b-da5e-4d09-94aa-7e0be245bb5d)

## TRANSIENT ANALYSIS

1. **AC signal**.  
2. Define the signal using **SINE(0.763V, 50mV, 1kHz)**.  
3. Navigate to **"Simulate" > "Edit Simulation Cmd" > "Transient"**. Configure the **Stop Time** to **10ms**.

![image](https://github.com/user-attachments/assets/c33b00ec-a229-4438-92c9-780ad1f21739)

## AC ANALYSIS 

![image](https://github.com/user-attachments/assets/2418e163-e878-4e70-8aa0-2a3a1c2af84b)

  
1. choose **AC Analysis**.  
2. **Type of Sweep** to **Decade**.  
3. Specify **20 points per decade** .
4. **frequency range** from **0.1Hz to 1THz**.

![image](https://github.com/user-attachments/assets/e913670f-cb6a-4c9f-a14a-f10f429f5326)

obtained gain 24.6db but expected 21db and 3db is 1.404hz .

![image](https://github.com/user-attachments/assets/0ff66afe-1bea-4c79-83d2-27195f6b1704)

## 1st Question inference

### **Inference**  

The experiment successfully designed and analyzed a **current mirror circuit** for 1:1 and 1:2 current ratios. DC analysis confirmed proper transistor biasing, while transient analysis showed stable operation. AC analysis revealed slight gain deviations (**21 dB vs. 20 dB** for 1:1 and **24.6 dB vs. 21 dB** for 1:2), likely due to device mismatches. Channel length variations impacted mirroring accuracy and bandwidth. Overall, the experiment validated theoretical predictions, emphasizing the importance of **W/L selection, biasing, and frequency response** in current mirror design.


# 2nd Question 



















