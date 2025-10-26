# EEE4022F-Final-Year-Project  
**Transient Stability of Multi-Machine Power Systems with Hybrid HVDC Transmission Lines and Grid-Scale BESS**

## 📘 Overview  
This project investigates how **hybrid HVDC systems**—combining Line Commutated Converter (LCC) and Voltage Source Converter (VSC) technologies—and **grid-scale Battery Energy Storage Systems (BESS)** affect the **transient stability** of multimachine power systems.  
Using the IEEE 9-bus test system modeled in **DIgSILENT PowerFactory**, several fault and disturbance cases were simulated to evaluate how coordinated converter–storage control improves grid resilience and prevents cascading failures.

---

## 🎯 Objectives  
- Develop a detailed **IEEE 9-bus multimachine system** integrated with hybrid HVDC and BESS.  
- Implement **control structures** for HVDC converters and BESS to manage active and reactive power exchange.  
- Evaluate the impact on **Critical Clearing Time (CCT)**, **rotor-angle synchronism**, **voltage recovery**, and **frequency support**.  
- Compare results between conventional AC systems and those enhanced with **hybrid HVDC–BESS coordination**.

---

## ⚙️ Methodology  
1. **System Modeling**  
   - Modeled the IEEE 9-bus system in DIgSILENT PowerFactory.  
   - Added LCC–VSC hybrid HVDC transmission links and BESS units.  

2. **Controller Design**  
   - Implemented **VSC current and voltage control loops**, **LCC rectifier control**, and **BESS PQ/frequency control** using DIgSILENT DSL.  

3. **Simulation Scenarios**  
   - Performed fault, generator outage, and load variation tests to assess transient responses.  
   - Compared system performance before and after HVDC–BESS integration.  

4. **Performance Metrics**  
   - Rotor-angle and speed deviation  
   - Frequency and voltage recovery  
   - Active and reactive power oscillations  
   - Critical Clearing Time (CCT) extension  

---

## 🚀 How to Run Simulations  

### **Software Requirements**  
- **DIgSILENT PowerFactory 2023 or later**  
- MATLAB (optional, for data post-processing and plotting)  
- LaTeX (for generating plots and report figures)  

### **Steps**  
1. **Open Project File**  
   - Load the PowerFactory project folder named `HVDC_BESS_IEEE9` (if cloned, located under `/Simulation_Files/`).  

2. **Load Network Model**  
   - Open the `IEEE_9Bus_HybridHVDC` model under the *Network Models* folder.  

3. **Configure Controllers**  
   - Ensure the LCC, VSC, and BESS controllers are activated.  
   - Check the BESS parameters (capacity, SOC, droop constants) under *Composite Models*.  

4. **Run Case Studies**  
   - Select one of the predefined events:  
     - `Case1_1_Fault` – Line Fault (no HVDC/BESS)  
     - `Case2_1_Fault` – Line Fault (with HVDC/BESS)  
     - `Case2_3_LoadEvent` – Load Increase with BESS Response  
     - `Case2_4_Outage` – Transmission Outage Event  
   - Run **RMS Simulation** for each case and export plots (rotor angle, frequency, voltage).  

5. **Compare Results**  
   - Analyze CCT improvements, damping ratios, and post-fault recovery.  
   - MATLAB scripts provided in `/Analysis_Scripts/` can be used for quantitative analysis.

---

## 📊 Key Findings  
- **Hybrid HVDC** enhances power controllability and enables **dynamic fault isolation**.  
- **BESS** provides **fast frequency and voltage support**, stabilizing post-fault oscillations.  
- Their **coordinated control** extends the **Critical Clearing Time (CCT)** and significantly improves **rotor-angle stability**.  
- The combination presents a **cost-effective approach** for strengthening future renewable-dominated grids.  

---

## 🧠 Keywords  
Transient Stability • Multi-Machine Power Systems • Hybrid HVDC • LCC–VSC • BESS • DIgSILENT PowerFactory • Critical Clearing Time  

---

## 👤 Author  
**Nefthali Motonosi (MTNNKH001)**  
Department of Electrical Engineering  
University of Cape Town  
**Supervisor:** A/Prof David Oyedokun  
📅 *Submitted: October 23, 2025*  
