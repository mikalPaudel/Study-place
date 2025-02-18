### **📜 Electrical Machines – Formula Sheet 📜**  

This sheet contains key formulas for **Transformers, DC Machines, Induction Machines, Synchronous Machines, and Fractional Kilowatt Motors**.

---

## **1️⃣ Magnetic Circuits & Induction**  
- **Ohm’s Law for Magnetic Circuits**:
  
  $\[  \Phi = \frac{MMF}{Reluctance}\]$
  where **\( MMF = N I \)** (Magnetomotive force).
  
- **Reluctance**:
  
  $\[ \mathcal{R} = \frac{l}{\mu A}\]$
  
- **Hysteresis Loss (Steinmetz Equation)**:
  
  $\[P_h = \eta B_m^{1.6} f V\]$

- **Eddy Current Loss**:
  
  $\[P_e = k B_m^2 f^2 t^2 V\]$
 
- **Faraday’s Law of Electromagnetic Induction**:
   
  $\[ e = -N \frac{d\Phi}{dt}\]$

- **Force on a Current-Carrying Conductor**:
    
  $\[ F = BIL \sin \theta\]$

---

## **2️⃣ Transformers**  
- **EMF Equation**:  

  $\[  E = 4.44 f \Phi N\]$

- **Voltage Transformation Ratio**:  

  $\[  \frac{V_1}{V_2} = \frac{N_1}{N_2}\]$

- **Current Transformation Ratio**:  

  $\[  \frac{I_1}{I_2} = \frac{N_2}{N_1}\]$

- **Efficiency**:
  
  $\[\eta = \frac{\text{Output Power}}{\text{Input Power}} \times 100\%\]$

- **Voltage Regulation**:  

  $\[ VR = \frac{E_{\text{no-load}} - V_{\text{full-load}}}{V_{\text{full-load}}} \times 100\%\]$
 
- **Condition for Maximum Efficiency**:  

   $\[  I_2 R_2 = P_c\]$
  where $\( P_c \)$ = core loss.  

---

## **3️⃣ DC Machines**  
### **DC Generator**  
- **EMF Equation**:  

 $\[  E = \frac{P \Phi Z N}{60 A}\]$
  where:  
  - $\( P \) $= Number of poles  
  - $\( \Phi \)$ = Flux per pole (Wb)  
  - $\( Z \) $= Total conductors  
  - $\( N \)$ = Speed (RPM)  
  - $\( A \)$ = Parallel paths  

- **Power Equation**:  

 $\[  P = VI\]$


### **DC Motor**  
- **Torque Equation**:  

   $\[  T = \frac{P \Phi Z I_a}{2\pi A}\]$

- **Back EMF**:  

  $\[  E_b = V - I_a R_a\]$
  
- **Speed Equation**:  

   $\[  N \propto \frac{E_b}{\Phi}\]$
  
- **Efficiency**:  

  $\[  \eta = \frac{\text{Output Power}}{\text{Input Power}} \times 100\%\]$

---

## **4️⃣ Three-Phase Induction Machines**  
- **Synchronous Speed**:  

  $\[N_s = \frac{120 f}{P}\]$
  
- **Slip**:  

 $\[  S = \frac{N_s - N_r}{N_s} \times 100\%\]$

- **Rotor Frequency**:  

  $\[  f_r = S f\]$
  
- **Torque Equation**:  

  $\[  T = \frac{K s E^2}{R_2 + s X_2^2}\]$
  
- **Maximum Torque Condition**:  

 $\[  s = \frac{R_2}{X_2}  \]$

---

## **5️⃣ Three-Phase Synchronous Machines**  
### **Synchronous Generator (Alternator)**  
- **EMF Equation**:  

  $\[  E_{\text{ph}} = 4.44 f \Phi T_{\text{ph}} K_w\]$
  
  where:  
  - $\( T_{\text{ph}} \) $= Turns per phase  
  - $\( K_w \)$ = Winding factor  

- **Voltage Regulation**:  
  $\[  VR = \frac{E_{\text{no-load}} - V_{\text{full-load}}}{V_{\text{full-load}}} \times 100\%\]$

### **Synchronous Motor**  
- **Power Equation**:  

  $\[  P = \frac{3 V E_f}{X_s} \sin \delta\]$
  
- **Power Factor Control**:  

  $\[\cos \theta = \frac{P}{VI}\]$
  

---

### **6️⃣ Fractional Kilowatt Motors (Continued)**  
#### **Single-Phase Induction Motors**  
- **Power Factor Improvement Using Capacitor**:  

  $\[  C = \frac{I}{2 \pi f V} \]$
  
  where:
  - $\( C \)$ = capacitance in Farads  
  - $\( I \)$ = current in Amps  
  - $\( f \)$ = frequency in Hz  
  - $\( V \)$ = voltage in Volts

#### **Split-Phase Induction Motor**  
- **Starting Torque**:  

  $\[  T_{\text{start}} = \frac{V^2 R_{\text{start}}}{X_{\text{start}}}\]$
  
  where:
  - $\( R_{\text{start}} \) $= resistance of the start winding  
  - $\( X_{\text{start}} \)$ = reactance of the start winding  

#### **Capacitor-Start Induction Motor**  
- **Starting Torque**:  

  $\[  T_{\text{start}} = \frac{V^2}{(R^2 + X^2)}\]$

  where:
  - $\( R \) $= resistance of the windings  
  - $\( X \)$ = reactance of the motor  

#### **Capacitor-Run Motor**  
- **Efficiency**:  

  $\[  \eta = \frac{P_{\text{out}}}{P_{\text{in}}} \times 100\]$
  
  where:
  - $\( P_{\text{out}} \)$ = output mechanical power  
  - $\( P_{\text{in}} \)$ = input electrical power  

---

### **Special Machines**  
#### **Stepper Motor**  
- **Step Angle**:  

  $\[  \theta_{\text{step}} = \frac{360^\circ}{\text{Number of steps per revolution}}\]$
  

#### **Schrage Motor**  
- **Torque Equation**:  

  $\[  T = \frac{V \cdot I}{\omega}\]$

  where:
  - $\( \omega \)$ = angular velocity in rad/s

#### **Universal Motor**  
- **Speed Equation**:  

   $\[  N = \frac{V}{k \Phi}\]$
  
  where:
  - $\( k \)$ = constant depending on motor construction  
  - $\( \Phi \)$ = flux in the motor

#### **Servo Motor**  
- **Torque-Speed Characteristics**:  

  $\[  T = \frac{V}{R} \times \left(1 - \frac{N_r}{N_s}\right)\]$
  
  where:
  - $\( T \) $= torque  
  - $\( V \)$ = voltage  
  - $\( N_r \)$ = rotor speed  
  - $\( N_s \)$ = synchronous speed

---

### **🔹 Key Notes on Units 🔹**  
- **Voltage (V)** = Volt  
- **Current (I)** = Ampere  
- **Power (P)** = Watt  
- **Torque (T)** = Newton-meter  
- **Speed (N)** = RPM (Revolutions per minute)  
- **Flux (Φ)** = Weber  
- **Efficiency (η)** = Percentage

---
