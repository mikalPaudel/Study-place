# Electric Machine

### **1. Magnetic Circuits and Induction**  

#### **1.1 Magnetic Circuits**  
A **magnetic circuit** is a closed path through which magnetic flux flows. It is analogous to an electric circuit, where current flows through a closed path.  

- **Magnetomotive Force (MMF)**: Similar to voltage in an electric circuit, MMF is the force that drives magnetic flux. It is given by:  
  \[
  \text{MMF} = NI
  \]  
  where \( N \) is the number of turns and \( I \) is the current.

- **Magnetic Flux (\( \Phi \))**: The total magnetic field passing through a given area. Measured in **Weber (Wb)**.  

- **Magnetic Field Strength (\( H \))**: It is the magnetizing force applied to a material, given by:  
  \[
  H = \frac{NI}{l}
  \]  
  where \( l \) is the length of the magnetic path.  

- **Magnetic Flux Density (\( B \))**: It is the flux per unit area:  
  \[
  B = \mu H
  \]  
  where \( \mu \) is the permeability of the material.

#### **1.2 Ohm’s Law for Magnetic Circuits**  
The relationship between MMF, flux, and reluctance (\( \mathcal{R} \)) is analogous to Ohm's law:  
\[
\Phi = \frac{\text{MMF}}{\mathcal{R}}
\]
where \( \mathcal{R} = \frac{l}{\mu A} \) is the reluctance (opposition to magnetic flux).  

#### **1.3 Series and Parallel Magnetic Circuits**  
- In **series magnetic circuits**, the same magnetic flux flows through all elements.  
- In **parallel magnetic circuits**, the total flux is divided among multiple paths, similar to a parallel electrical circuit.

#### **1.4 Core with Air Gap**  
- When a core has an air gap, it introduces **high reluctance** because air has a much lower permeability than the core material.  
- Air gaps are used in machines to control the flux and prevent saturation.  

#### **1.5 B-H Relationship (Magnetization Characteristics)**  
- The **B-H curve** shows the relationship between **magnetic field strength (H)** and **magnetic flux density (B)**.
- Ferromagnetic materials exhibit **non-linearity**, meaning \( B \) does not increase proportionally with \( H \) due to **saturation**.

#### **1.6 Hysteresis with DC and AC Excitation**  
- When a magnetic material is subjected to a varying magnetic field, the flux lags behind the applied field, forming a **hysteresis loop**.
- **DC excitation** results in a single loop.
- **AC excitation** causes continuous cycles of magnetization and demagnetization.

#### **1.7 Hysteresis Loss and Eddy Current Loss**  
- **Hysteresis Loss**: Energy lost due to repeated magnetization and demagnetization. It depends on the area of the hysteresis loop.  
  \[
  P_h = \eta B_{\max}^{1.6} f V
  \]
  where \( \eta \) is a material-dependent constant, \( f \) is frequency, and \( V \) is volume.  
- **Eddy Current Loss**: Circulating currents (eddy currents) are induced in the core due to changing magnetic fields, leading to power loss.  
  \[
  P_e = k B_{\max}^2 f^2 t^2 V
  \]
  where \( t \) is the thickness of the core.

#### **1.8 Faraday’s Law of Electromagnetic Induction**  
1. **First Law**: A time-varying magnetic field induces an **EMF** in a coil.
2. **Second Law**: The magnitude of induced EMF is proportional to the rate of change of flux:  
   \[
   e = -N \frac{d\Phi}{dt}
   \]  
   (negative sign due to Lenz’s Law).

#### **1.9 Statically and Dynamically Induced EMF**  
- **Statically Induced EMF**: When flux linking a coil changes but the conductor remains stationary.  
  - Example: Transformer action.  
- **Dynamically Induced EMF**: When a conductor moves through a magnetic field.  
  - Example: EMF generated in a rotating machine.

#### **1.10 Force on Current Carrying Conductor**  
A current-carrying conductor in a magnetic field experiences a force given by **Lorentz Force Law**:  
\[
F = BIL \sin \theta
\]  
where \( B \) is the flux density, \( I \) is the current, and \( L \) is the length of the conductor.

---

### **2. Transformer**  

A **transformer** is a static electrical device that transfers electrical energy between circuits through electromagnetic induction. It operates on **AC supply** and is used for voltage transformation in power systems.  

---

### **2.1 Constructional Details and Recent Trends**  
A transformer consists of:  
- **Core**: Made of laminated silicon steel to minimize **eddy current losses**.  
- **Windings**:  
  - **Primary winding** (connected to the input source).  
  - **Secondary winding** (connected to the output load).  
- **Insulation**: Separates windings to prevent short circuits.  
- **Cooling System**:  
  - **Air-cooled (dry-type)** for small transformers.  
  - **Oil-cooled** for large transformers (immersed in insulating oil).  

👉 **Recent Trends**:  
- **Amorphous Core Transformers**: Uses amorphous metal to reduce core losses.  
- **Smart Transformers**: Integrated with **IoT** for real-time monitoring.  
- **Solid-State Transformers**: Uses **power electronics** for advanced control.  

---

### **2.2 Working Principle and EMF Equation**  
A transformer works on **Faraday’s Law of Electromagnetic Induction**:  
\[
e = -N \frac{d\Phi}{dt}
\]  
When AC voltage is applied to the primary winding, it creates a **changing magnetic flux**, which induces voltage in the secondary winding.  

#### **EMF Equation of a Transformer**  
\[
E = 4.44 f N \Phi_m
\]
where,  
- \( E \) = Induced EMF (V)  
- \( f \) = Supply frequency (Hz)  
- \( N \) = Number of turns  
- \( \Phi_m \) = Maximum flux (Weber)  

For primary and secondary windings:  
\[
E_1 = 4.44 f N_1 \Phi_m, \quad E_2 = 4.44 f N_2 \Phi_m
\]  
Thus, the **turns ratio** is:  
\[
\frac{E_2}{E_1} = \frac{N_2}{N_1}
\]  
- **Step-up Transformer**: \( N_2 > N_1 \) (increases voltage).  
- **Step-down Transformer**: \( N_2 < N_1 \) (decreases voltage).  

---

### **2.3 Ideal Transformer**  
An **ideal transformer** assumes:  
- **Zero losses** (no core loss, no copper loss).  
- **100% efficiency**.  
- **Magnetizing current is negligible**.  

For an ideal transformer:  
\[
V_1 I_1 = V_2 I_2
\]  
where \( V_1, I_1 \) are primary voltage and current, and \( V_2, I_2 \) are secondary voltage and current.  

---

### **2.4 No-Load and Load Operation**  
#### **No-Load Operation**  
- Secondary winding **open**, primary winding connected to AC supply.  
- Small **magnetizing current** flows in the primary to establish flux.  
- No-load current **lags** applied voltage by \( 80^\circ - 85^\circ \).  

#### **Load Operation**  
- When a load is connected, secondary winding **draws current**.  
- The primary winding adjusts to maintain flux balance.  
- Power is transferred from primary to secondary.  

---

### **2.5 Equivalent Circuit and Phasor Diagram**  
The practical transformer has losses and is represented by an **equivalent circuit**.  

#### **Equivalent Circuit**  
\[
\begin{aligned}
    R_1, R_2 & : \text{Primary and secondary resistance (copper loss).} \\
    X_1, X_2 & : \text{Primary and secondary leakage reactance.} \\
    R_c & : \text{Core loss resistance (hysteresis + eddy current loss).} \\
    X_m & : \text{Magnetizing reactance (required to establish flux).}
\end{aligned}
\]

By referring the secondary values to the primary, we get:  
\[
R_2' = \left(\frac{N_1}{N_2}\right)^2 R_2, \quad X_2' = \left(\frac{N_1}{N_2}\right)^2 X_2
\]

---

### **2.6 Transformer Tests**  
To determine equivalent circuit parameters, we perform:  

1️⃣ **Polarity Test**: Determines relative polarity of windings (helps in parallel operation).  

2️⃣ **Open Circuit Test** (O.C. Test):  
- Secondary is **open**, primary is supplied rated voltage.  
- Measures **core loss (iron loss)**.  

3️⃣ **Short Circuit Test** (S.C. Test):  
- Primary is **shorted**, secondary supplied with reduced voltage.  
- Measures **copper loss** and impedance.  

---

### **2.7 Voltage Regulation**  
Voltage regulation measures how much the output voltage changes with load:  
\[
\% \text{Regulation} = \frac{V_{nl} - V_{fl}}{V_{fl}} \times 100
\]  
where:  
- \( V_{nl} \) = No-load voltage  
- \( V_{fl} \) = Full-load voltage  

A good transformer has **low voltage regulation** (less voltage drop).  

---

### **2.8 Losses in a Transformer and Efficiency**  
Total loss = **Copper loss** + **Iron loss**  

1. **Copper Loss** (\( I^2R \)):  
   \[
   P_c = I_1^2 R_1 + I_2^2 R_2
   \]  
2. **Iron Loss**:  
   - **Hysteresis Loss** \( P_h = k B_{\max}^{1.6} f V \)  
   - **Eddy Current Loss** \( P_e = k B_{\max}^2 f^2 t^2 V \)  

#### **Efficiency of Transformer**  
\[
\eta = \frac{\text{Output Power}}{\text{Input Power}} \times 100
\]  
For **maximum efficiency**:  
\[
P_c = P_i
\]  

#### **All-Day Efficiency**  
\[
\eta_{\text{all-day}} = \frac{\text{Total Output Energy}}{\text{Total Input Energy}} \times 100
\]  
Used for **distribution transformers** where iron loss dominates.  

---

### **2.9 Instrument Transformers**  
1. **Potential Transformer (PT)**: Steps down high voltage for metering.  
2. **Current Transformer (CT)**: Steps down high current for measurement.  

---

### **2.10 Auto Transformer**  
An **autotransformer** has a single winding with a tapping point:  
\[
\frac{V_2}{V_1} = \frac{N_2}{N_1}
\]  
✔️ **Copper Saving**:  
\[
\text{Cu Saving} = 1 - \frac{V_2}{V_1}
\]  
Uses: **Voltage regulation, motor starting, and railway traction**.  

---

### **2.11 Three-Phase Transformers**  
- Built as **three single-phase units** or a **single three-phase unit**.  
- **Connections**:  
  - **Star-Star (Y-Y)**: Used for high-voltage transmission.  
  - **Delta-Delta (Δ-Δ)**: Used for industrial applications.  
  - **Star-Delta (Y-Δ)**: Used in power systems.  

---

### **3. DC Generator**  

A **DC generator** converts **mechanical energy** into **electrical energy** using the principle of **electromagnetic induction**. It generates **direct current (DC)** output.  

---

### **3.1 Constructional Details and Armature Winding**  
A **DC generator** consists of:  

1️⃣ **Yoke**: Provides mechanical support and acts as a **magnetic path**.  
2️⃣ **Pole Core & Pole Shoes**: Distribute the **magnetic flux** uniformly.  
3️⃣ **Field Winding**: Produces the required **magnetic field** (excitation).  
4️⃣ **Armature Core**:  
   - Laminated to **reduce eddy current losses**.  
   - Provides a path for magnetic flux.  
5️⃣ **Armature Winding**:  
   - Carries **induced EMF** and **current**.  
   - **Types of winding**:  
     - **Lap Winding**: Used in **high current, low voltage** machines.  
     - **Wave Winding**: Used in **high voltage, low current** machines.  
6️⃣ **Commutator**: Converts **AC induced EMF** into **DC output**.  
7️⃣ **Brushes**: Conduct current from **commutator to external circuit**.  

---

### **3.2 Working Principle and Commutator Action**  
A DC generator works on **Faraday’s Law of Electromagnetic Induction**:  
\[
e = -N \frac{d\Phi}{dt}
\]  
When the **armature rotates** in a magnetic field, **EMF is induced** in the windings.  

#### **Commutator Action**  
- The generated EMF in the armature winding is **AC**.  
- The **commutator** converts AC into **DC** by reversing the connections at every half-cycle.  
- The brushes maintain a **unidirectional current flow**.  

---

### **3.3 EMF Equation of a DC Generator**  
\[
E = \frac{P \Phi Z N}{60 A}
\]  
where,  
- \( P \) = Number of poles  
- \( \Phi \) = Flux per pole (Weber)  
- \( Z \) = Total armature conductors  
- \( N \) = Speed in RPM  
- \( A \) = Number of parallel paths (\( A = P \) for lap winding, \( A = 2 \) for wave winding)  

---

### **3.4 Methods of Excitation & Types of DC Generators**  
**Excitation** refers to the method of supplying current to the **field winding**.  

1️⃣ **Separately Excited DC Generator**  
   - Field winding gets power from an **external source**.  

2️⃣ **Self-Excited DC Generator**  
   - Field winding gets power from the generator itself.  
   - Types:  
     - **Series Generator**: Field winding in **series** with armature.  
     - **Shunt Generator**: Field winding in **parallel** with armature.  
     - **Compound Generator**: **Combination of series and shunt winding**.  
       - **Cumulative Compound**: Series field aids shunt field.  
       - **Differential Compound**: Series field opposes shunt field.  

---

### **3.5 Characteristics of DC Generators**  
1️⃣ **Open Circuit Characteristic (OCC)**:  
   - Shows how **induced EMF** varies with field current **at no load**.  
   - Initially, **EMF increases linearly**, then saturates.  

2️⃣ **Internal Characteristic (E vs. Ia)**:  
   - Shows variation of **generated EMF (E)** with **armature current (Ia)**.  

3️⃣ **External Characteristic (V vs. IL)**:  
   - Shows how **terminal voltage (V)** varies with **load current (IL)**.  

---

### **3.6 Losses in DC Generators**  
**Total Loss = Copper Loss + Iron Loss + Mechanical Loss**  

1️⃣ **Copper Loss**  
   - **Armature Copper Loss** \( P_{cu} = I_a^2 R_a \)  
   - **Field Copper Loss** \( P_f = I_f^2 R_f \)  

2️⃣ **Iron Loss (Core Loss)**  
   - **Hysteresis Loss** \( P_h = k B_{\max}^{1.6} f V \)  
   - **Eddy Current Loss** \( P_e = k B_{\max}^2 f^2 t^2 V \)  

3️⃣ **Mechanical Loss**  
   - **Friction Loss** (bearings, brushes).  
   - **Windage Loss** (air resistance).  

---

### **3.7 Efficiency & Voltage Regulation**  
#### **Efficiency of a DC Generator**  
\[
\eta = \frac{\text{Output Power}}{\text{Input Power}} \times 100
\]  

For **maximum efficiency**:  
\[
\text{Variable Loss} = \text{Constant Loss}
\]  

#### **Voltage Regulation**  
\[
\% \text{Regulation} = \frac{V_{no-load} - V_{full-load}}{V_{full-load}} \times 100
\]  
- **Good regulation** means less voltage drop.  

---

### **4. DC Motors**  

A **DC motor** converts **electrical energy** into **mechanical energy** based on the principle of **Lorentz Force**, where a current-carrying conductor experiences a force when placed in a magnetic field.  

---

### **4.1 Working Principle & Torque Equation**  
A DC motor operates on **Faraday’s Law of Induction** and **Lorentz Force Law**:  
\[
F = BIL \sin \theta
\]  
where,  
- \( F \) = Force on the conductor (N)  
- \( B \) = Magnetic flux density (T)  
- \( I \) = Current in the conductor (A)  
- \( L \) = Length of the conductor in the field (m)  
- \( \theta \) = Angle between the conductor and magnetic field  

The force produces **torque** in the rotor, causing it to rotate.  

#### **Torque Equation of a DC Motor**  
\[
T = \frac{P Z}{2\pi A} \Phi I_a
\]  
where,  
- \( T \) = Torque (N·m)  
- \( P \) = Number of poles  
- \( Z \) = Total armature conductors  
- \( A \) = Number of parallel paths  
- \( \Phi \) = Magnetic flux per pole (Wb)  
- \( I_a \) = Armature current (A)  

---

### **4.2 Back EMF (Counter EMF)**  
When the motor starts rotating, the armature conductors **cut the magnetic field**, inducing an **opposing EMF** called **Back EMF (\(E_b\))**, given by:  
\[
E_b = \frac{P \Phi Z N}{60 A}
\]  
where, \( N \) is the speed in RPM.  

Since **back EMF opposes the supply voltage**, the actual voltage across the armature is:  
\[
V = E_b + I_a R_a
\]  

- At **starting**, \( E_b = 0 \), so **high current** flows, requiring a **starter**.  
- As the motor speeds up, \( E_b \) **increases** and limits the current.  

---

### **4.3 Methods of Excitation & Types of DC Motors**  

DC motors are classified based on **how the field winding is excited**:  

1️⃣ **Separately Excited DC Motor**  
   - Field winding gets power from an **external source**.  

2️⃣ **Self-Excited DC Motor**  
   - Field winding is powered by the motor itself.  
   - **Types**:  
     - **Series Motor**: Field winding in **series** with armature.  
     - **Shunt Motor**: Field winding in **parallel** with armature.  
     - **Compound Motor**: Has **both series & shunt** windings.  
       - **Cumulative Compound**: Series field **aids** shunt field.  
       - **Differential Compound**: Series field **opposes** shunt field.  

---

### **4.4 Performance Characteristics of DC Motors**  
1️⃣ **Torque vs. Armature Current**  
   - **Series Motor**: **Steep** increase (high starting torque).  
   - **Shunt Motor**: **Linear** increase.  
   - **Compound Motor**: **Intermediate** behavior.  

2️⃣ **Speed vs. Armature Current**  
   - **Series Motor**: Speed **drops** as load increases.  
   - **Shunt Motor**: Almost **constant speed**.  
   - **Compound Motor**: **Moderate** speed drop.  

3️⃣ **Speed vs. Torque**  
   - **Series Motor**: **Very high torque at low speeds** (used in cranes, electric trains).  
   - **Shunt Motor**: **Constant torque** (used in lathes, fans).  
   - **Compound Motor**: **Moderate characteristics** (used in lifts, compressors).  

---

### **4.5 Starting of DC Motors**  

Since **starting current is very high**, a **starter** is used to protect the motor.  

#### **Types of Starters**  
1️⃣ **Three-Point Starter** (for Shunt & Compound Motors)  
   - Contains **Overload Protection** and **No-Voltage Protection**.  
   - Uses a **starting resistance** that is gradually reduced.  

2️⃣ **Four-Point Starter**  
   - More **stable** than a three-point starter.  
   - Independent of **field circuit fluctuations**.  

---

### **4.6 Speed Control of DC Motors**  
Speed (\( N \)) of a DC motor is given by:  
\[
N = \frac{V - I_a R_a}{K \Phi}
\]  

#### **Methods of Speed Control**  
1️⃣ **Field Control (for Shunt & Compound Motors)**  
   - Vary **flux (\(\Phi\))** by changing field current.  
   - **Increasing \( R_f \)** → **Decreases \( \Phi \)** → **Increases speed**.  

2️⃣ **Armature Control (for Series & Shunt Motors)**  
   - Vary **voltage across armature** using a variable resistor.  
   - **Higher voltage → Higher speed**.  

3️⃣ **Voltage Control (for Series Motors)**  
   - Supply voltage is varied using **tapped resistors or chopper circuits**.  

---

### **4.7 Losses & Efficiency of DC Motors**  

#### **Types of Losses**  
1️⃣ **Copper Loss**  
   - \( P_{cu} = I_a^2 R_a \) (Armature Copper Loss)  
   - \( P_f = I_f^2 R_f \) (Field Copper Loss)  

2️⃣ **Iron Loss (Core Loss)**  
   - **Hysteresis Loss** \( P_h = k B_{\max}^{1.6} f V \)  
   - **Eddy Current Loss** \( P_e = k B_{\max}^2 f^2 t^2 V \)  

3️⃣ **Mechanical Loss**  
   - **Friction Loss** (bearings, brushes).  
   - **Windage Loss** (air resistance).  

#### **Efficiency of a DC Motor**  
\[
\eta = \frac{\text{Output Power}}{\text{Input Power}} \times 100
\]  
For **maximum efficiency**:  
\[
\text{Variable Loss} = \text{Constant Loss}
\]  

---

### **Key Applications of DC Motors**  

| **Motor Type** | **Applications** |
|--------------|-----------------|
| **Series Motor** | Electric trains, Cranes, Elevators, Hoists |
| **Shunt Motor** | Fans, Lathes, Blowers, Conveyors |
| **Compound Motor** | Rolling mills, Compressors, Punching machines |

---

### **5. Three-Phase Induction Machines**  

An **Induction Machine** is an **AC motor** that operates on the principle of **electromagnetic induction**. It is the most widely used motor due to its **ruggedness, simplicity, and low maintenance**.  

---

### **5.1 Three-Phase Induction Motor**  

A **three-phase induction motor** consists of:  
1️⃣ **Stator** – The stationary part that produces a **rotating magnetic field (RMF)**.  
2️⃣ **Rotor** – The rotating part, where EMF is induced due to **Faraday’s Law**.  

---

### **5.2 Construction & Types**  

🔹 **Stator**  
- Made of **laminated iron core** to reduce eddy current losses.  
- **Three-phase windings** are placed in **slots** at **120° apart** to create an RMF.  

🔹 **Rotor Types**  
1️⃣ **Squirrel Cage Rotor**  
   - Most common, simple, rugged, and low maintenance.  
   - Conductors are **short-circuited** using **end rings**.  
   - Used in **fans, pumps, blowers, and industrial machines**.  

2️⃣ **Wound Rotor (Slip Ring Rotor)**  
   - Has **three-phase windings** connected to **slip rings**.  
   - Used for **variable speed applications** (cranes, lifts, compressors).  

---

### **5.3 Operating Principle**  
- When a **three-phase AC supply** is given to the stator, a **rotating magnetic field (RMF)** is produced.  
- Due to **electromagnetic induction**, EMF is induced in the rotor conductors.  
- Since the rotor is **short-circuited**, a **current flows**, producing torque due to **Lorentz force**.  
- The rotor **tries to catch up with the RMF** but never reaches it.  

---

### **5.4 Rotating Magnetic Field (RMF)**  
The stator produces an RMF whose speed is called **synchronous speed (\( N_s \))**, given by:  
\[
N_s = \frac{120 f}{P}
\]  
where,  
- \( f \) = Supply frequency (Hz)  
- \( P \) = Number of poles  

---

### **5.5 Slip (\( S \))**  
Since the rotor **never reaches synchronous speed**, we define **slip** as:  
\[
S = \frac{N_s - N_r}{N_s} \times 100\%
\]  
where,  
- \( N_s \) = Synchronous speed (RPM)  
- \( N_r \) = Rotor speed (RPM)  

- **At start**, \( S = 1 \) (100% slip).  
- **During operation**, \( S \) is **small (~0.2% to 6%)**.  

---

### **5.6 Induced EMF & Rotor Current Frequency**  
By **Faraday’s Law**, the rotor EMF is:  
\[
E_2 = SE_s
\]  
where \( E_s \) is the stator voltage.  

Rotor current frequency:  
\[
f_r = S f
\]  
At full speed, \( f_r \) is **very small** (~2 Hz for 50 Hz supply).  

---

### **5.7 Torque Equation**  
The torque developed is given by:  
\[
T = \frac{K S E_2^2}{R_2 + S X_2}
\]  
where,  
- \( K \) = Constant  
- \( R_2 \) = Rotor resistance  
- \( X_2 \) = Rotor reactance  

- **High slip → High torque** (start-up).  
- **Low slip → Constant speed** (normal operation).  

---

### **5.8 Torque-Slip Characteristics**  
- **At start (\( S = 1 \))**, torque is **high**.  
- **As slip decreases**, torque **increases**, reaches **maximum (Breakdown Torque)**, and then **decreases**.  
- **Stable operation** is in the **low slip region (1-6%)**.  

---

### **5.9 Three-Phase Induction Generator**  
- Works like an **Induction Motor** but in **reverse**.  
- Used in **wind power plants** and **small hydro-power systems**.  
- Requires an **external reactive power source** to maintain excitation.  

**Voltage Build-up Condition:**  
1️⃣ Needs **residual magnetism**.  
2️⃣ Requires **capacitor bank** for reactive power.  
3️⃣ Operates at **negative slip (S < 0)**.  

---

### **5.10 Power Stages in an Induction Motor**  
The power flow in an Induction Motor is:  

1️⃣ **Input Power**:  
\[
P_{\text{input}} = \sqrt{3} V_L I_L \cos\phi
\]  

2️⃣ **Stator Copper & Core Losses**:  
\[
P_{\text{stator}} = P_{\text{input}} - P_{\text{stator losses}}
\]  

3️⃣ **Rotor Input Power**:  
\[
P_{\text{rotor input}} = P_{\text{stator}} - P_{\text{core loss}}
\]  

4️⃣ **Rotor Copper Losses**:  
\[
P_{\text{rotor copper loss}} = S P_{\text{rotor input}}
\]  

5️⃣ **Mechanical Power Output**:  
\[
P_{\text{mechanical}} = (1 - S) P_{\text{rotor input}}
\]  

6️⃣ **Shaft Power Output**:  
\[
P_{\text{output}} = P_{\text{mechanical}} - P_{\text{friction loss}}
\]  

#### **Efficiency**  
\[
\eta = \frac{P_{\text{output}}}{P_{\text{input}}} \times 100
\]  

---

### **Applications of Three-Phase Induction Motors**  

| **Motor Type** | **Applications** |
|---------------|-----------------|
| **Squirrel Cage Motor** | Fans, Pumps, Compressors, Blowers |
| **Slip Ring Motor** | Crushers, Hoists, Lifts, Rolling Mills |

---

### **6. Three-Phase Synchronous Machines**  

A **Synchronous Machine** is an AC machine where the rotor rotates at the same speed as the stator’s **rotating magnetic field (RMF)**. It can operate as a **Generator (Alternator)** or a **Motor**.

---

## **6.1 Three-Phase Synchronous Generator (Alternator)**  

A **Synchronous Generator** converts **mechanical energy (from turbines) into electrical energy** using **Faraday’s Law of Electromagnetic Induction**.

### **6.1.1 Constructional Details**  
1️⃣ **Stator** – Contains **armature windings** where EMF is induced.  
2️⃣ **Rotor** – Produces a magnetic field using **field windings** and a **DC exciter**.  
3️⃣ **Excitation System** – Provides **DC supply** to the rotor to maintain magnetic flux.  

🔹 **Types of Rotor**  
- **Salient Pole Rotor** – Used in **low-speed applications** (hydropower).  
- **Cylindrical Rotor (Smooth Rotor)** – Used in **high-speed applications** (thermal power plants).  

---

### **6.1.2 Working Principle**  
- A **prime mover** (turbine) rotates the rotor, producing a **rotating magnetic field**.  
- Due to **Faraday’s Law**, EMF is **induced** in the stator windings.  
- The frequency of generated EMF is:  
  \[
  f = \frac{PN}{120}
  \]  
  where:  
  - \( P \) = Number of poles  
  - \( N \) = Rotor speed (RPM)  

---

### **6.1.3 EMF Equation**  
\[
E_{\text{ph}} = 4.44 f \phi T_{\text{ph}} K_w
\]  
where:  
- \( E_{\text{ph}} \) = Generated EMF per phase  
- \( f \) = Frequency (Hz)  
- \( \phi \) = Flux per pole (Wb)  
- \( T_{\text{ph}} \) = Turns per phase  
- \( K_w \) = Winding factor  

---

### **6.1.4 Armature Reaction**  
- **At Unity Power Factor** → Purely **resistive**, no effect.  
- **At Lagging Power Factor** → Magnetic field is **weakened** (Demagnetizing).  
- **At Leading Power Factor** → Magnetic field is **strengthened** (Magnetizing).  

---

### **6.1.5 Synchronous Generator with Load**  
- When a load is connected, the **phasor diagram** changes based on power factor.  
- **Voltage Regulation (\( VR \))** is given by:  
  \[
  VR = \frac{E_{\text{no-load}} - V_{\text{full-load}}}{V_{\text{full-load}}} \times 100\%
  \]  

---

## **6.2 Three-Phase Synchronous Motor**  
A **Synchronous Motor** is a **constant-speed motor** that runs at synchronous speed.

---

### **6.2.1 Principle of Operation**  
- **Stator** produces a **rotating magnetic field**.  
- **Rotor** is magnetized by a **DC source** and locks with the RMF.  
- The motor operates at **synchronous speed (\( N_s \))**.  

\[
N_s = \frac{120 f}{P}
\]  

---

### **6.2.2 Starting Methods**  
A Synchronous Motor **cannot start on its own** because:  
- The rotor is **not initially rotating**.  
- The RMF is **too fast** for the rotor to catch up.  

🔹 **Starting Methods:**  
1️⃣ **Using an Induction Motor** (Rotor starts as an Induction Motor).  
2️⃣ **Damper Windings** (Provide starting torque).  

---

### **6.2.3 Effect of Excitation on Power Factor**  
- **Under-excited** → **Lagging Power Factor**  
- **Over-excited** → **Leading Power Factor** (Used for **power factor correction**).  
- **Correctly excited** → **Unity Power Factor**  

---

### **6.2.4 Applications of Synchronous Machines**  

| **Type** | **Application** |
|----------|---------------|
| **Synchronous Generator** | Power plants (Hydro, Thermal, Nuclear) |
| **Synchronous Motor** | Power factor correction, Large industrial loads |

---

### **7. Fractional Kilowatt Motors**  

Fractional Kilowatt (FKW) Motors are **small electrical motors** with a power rating **less than 1 kW**. They are widely used in **household appliances, office equipment, and industrial automation**.  

---

## **7.1 Single-Phase Induction Motors**  
A **Single-Phase Induction Motor** operates on a **single-phase AC supply**. Unlike three-phase motors, they **cannot self-start** because they lack a rotating magnetic field.  

### **7.1.1 Construction and Characteristics**  
🔹 **Stator** → Has a **single-phase winding** that produces an **oscillating** magnetic field.  
🔹 **Rotor** → Squirrel cage rotor similar to a three-phase induction motor.  
🔹 **Auxiliary Winding** → Used for starting the motor.  

---

### **7.1.2 Double-Field Revolving Theory**  
Since a single-phase AC supply produces an **alternating** (not rotating) magnetic field, it can be mathematically considered as:  
\[
\Phi_{\text{single-phase}} = \Phi_{\text{forward}} + \Phi_{\text{backward}}
\]  
where:  
- **Forward field** rotates in the same direction as the rotor.  
- **Backward field** rotates in the opposite direction.  

At standstill, these two fields **cancel each other**, preventing self-starting.

---

## **7.2 Types of Single-Phase Induction Motors**  
To overcome the starting problem, auxiliary methods are used.

### **7.2.1 Split-Phase Induction Motor**  
✅ Uses an additional **starting winding** with a **series resistor** to create a phase shift.  
✅ When the motor reaches **75% of synchronous speed**, the starting winding is disconnected.  
✅ **Application:** Fans, blowers, washing machines.

---

### **7.2.2 Capacitor-Start Induction Motor**  
✅ Uses a **capacitor in series** with the starting winding to improve starting torque.  
✅ Once started, a centrifugal switch disconnects the capacitor.  
✅ **Application:** Air compressors, pumps, refrigerators.

---

### **7.2.3 Capacitor-Start and Run Induction Motor**  
✅ Uses **two capacitors**, one for starting and one for running.  
✅ Provides **high starting torque** and **better efficiency**.  
✅ **Application:** Air conditioners, refrigeration units.

---

### **7.2.4 Reluctance-Start Induction Motor**  
✅ Has **special rotor slots** to create additional torque.  
✅ **Application:** Small fans, record players.

---

## **7.3 Alternating Current (AC) Series Motor and Universal Motor**  
These motors can **run on both AC and DC supplies**.  

🔹 **AC Series Motor** → Similar to a DC series motor but adapted for AC.  
🔹 **Universal Motor** → Works on both AC and DC due to **series excitation**.  
🔹 **Application:** Hand drills, sewing machines, vacuum cleaners.

---

## **7.4 Special Purpose Machines**  
### **7.4.1 Stepper Motor**  
✅ A **digital motor** that moves in **discrete steps**.  
✅ Used in **robotics, CNC machines, and printers**.  

### **7.4.2 Schrage Motor**  
✅ Variable-speed motor used in **textile mills**.  

### **7.4.3 Servo Motor**  
✅ Precision motor with **position control**.  
✅ Used in **robotics and automation**.  

---

### **Conclusion**  
Fractional Kilowatt Motors are essential in various applications, from **home appliances** to **industrial automation**.  


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
