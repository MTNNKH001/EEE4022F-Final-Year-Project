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

### **Steps**  
1. **Open Project File**  
   - Import DIgSILENT PowerFactory file named "IEEE 9 bus Hybrid HVDC and BESS_1"
2. **Load Network Model**  
   - Activate the project file "IEEE 9 bus Hybrid HVDC and BESS_1"

3. **Run Case Studies**  
   - Activate case study you intend to test 
   - Run **RMS/EMT Simulation** for each case and see plots.  

5. **Compare Results**  
   - Analyze CCT improvements, damping ratios, and post-fault recovery. 

---

## 📊 Key Findings  
- **Hybrid HVDC** enhances power controllability and enables **dynamic fault isolation**.  
- **BESS** provides **fast frequency and voltage support**, stabilizing post-fault oscillations.  
- Their **coordinated control** extends the **Critical Clearing Time (CCT)** and significantly improves **rotor-angle stability**.  
- The combination presents a **cost-effective approach** for strengthening future renewable-dominated grids.  

---

## 🧠 Keywords  
Transient Stability • Multi-Machine Power Systems • Hybrid HVDC • LCC–VSC • BESS
---

## 👤 Author  
**Nefthali Motonosi (MTNNKH001)**  
Department of Electrical Engineering  
University of Cape Town
