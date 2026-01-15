# **Genaro Salazar Ruiz**
### Systems-Level Embedded & RF Engineer 📡⚡️

---

## **Professional Summary**

Electrical Engineer and M.S. candidate in **Wireless Embedded Systems** (UC San Diego, 2027) specializing in **embedded firmware, RF systems, and real-time DSP/control**.  

Over **three years of hands-on experience** building and optimizing hardware-driven systems — from low-power oceanographic platforms to precision RF synthesizers.  

Focused on **deterministic performance**, **signal-chain optimization**, and **cross-domain system integration**, bridging hardware, firmware, and test automation.  

> Design at the intersection of timing, power, and precision.

---

## **Technical Proficiencies**

| Category | Core Strengths |
|:--|:--|
| **Languages** | C, C++, Python, MATLAB, Armv8 Assembly |
| **Embedded Systems** | DMA, ISR, Low-Power (EMx), Real-Time Control (PID), Sensor Integration, PCB Design |
| **RF / DSP** | PLLs (Integer-N/Fractional-N), Fixed-Point Q16.16, Phase Tracking, Loop Filter Design |
| **Platforms** | EFM32, LMX2820, STM32, MSP430, ESP32, Raspberry Pi |
| **Tools & Frameworks** | Git, VSCode, PySerial, CCStudio, Test Automation (Python/SCPI) |

---

## **Flagship Engineering Projects**

Precision-built systems demonstrating control-loop accuracy, power optimization, and validated hardware interfacing.

---

### 🔋 **1. Low-Power DMA UART Logger – Multiscale Ocean Dynamics**  
**Repository:** [Low-Power-Logger](https://github.com/pollo2001/Low-Power-Logger)  
**Context:** Firmware developed for **UCSD’s Multiscale Ocean Dynamics Lab**, supporting extended oceanographic research deployments.  
- Architected a **DMA-driven UART logging framework** allowing the MCU to remain in deep-sleep (EM2) while maintaining microsecond-level timing.  
- Achieved **>90% power reduction** through interrupt-based packet collection and peripheral wake-on-UART design.  
- Validated on **field-deployed sensor platforms** requiring deterministic timing and multi-day uptime.  
- **NDA-compliant sanitized release.**


**Skills:** C, EFM32 Firmware, DMA, ISR, Low-Power Embedded Design, Real-Time Logging  

---

### 📡 **2. RF Synthesizer Test Automation Framework – Z-Communications, Inc.**  
**Repository:** [Smart_PLL_Interface](https://github.com/pollo2001/Smart_PLL_Interface)  
**Context:** Developed a **Python-based GUI test automation suite** for Z-Comm’s Smart SSG PLL synthesizer line.  
- Created a **multi-threaded, SCPI-style control layer** for real-time PLL characterization and validation.  
- Automated frequency sweeps, lock-time verification, and phase-noise measurement routines.  
- Reduced manual test time by over **60%**, accelerating hardware validation cycles.
-  NDA Compliant

**Skills:** Python, GUI Development, Serial Communication, RF Control, SCPI Automation  

---


### ⚡ **3. Three-Wire SPI Bit-Bang – PLL Synthesizer Initialization - Z-Communications, Inc.**
**Repository:** [NDA-Generic-BitBang-OneTime](https://github.com/pollo2001/NDA-Generic-BitBang-OneTime)
**Context**: Designed a compact bit-bang SPI implementation to program a **PLL frequency synthesizer** on an MSP430, where hardware SPI lines were unavailable due to board constraints.  
- Implemented three-wire protocol (DATA, CLK, LE) for 24-bit register writes to configure PLL dividers, charge pump settings, and reference frequency.
- Prioritized simplicity over speed — one-time initialization negated the need for a hardware SPI peripheral, reducing pin conflicts and firmware complexity.
- MCU enters deep sleep (LPM4) after initialization to minimize current draw and ensure brownout safety during RF operation.
- NDA-compliant release preserving protocol logic without exposing proprietary register maps.

**Skills:** Embedded C, Bit-Bang SPI, MSP430, RF Synthesizer Programming, Low-Power Design, Hardware Constraint Solving

---

### ⚙️ **4. BareMetalPLL – Digital Phase-Locked Loop Simulation (C)**  
**Repository:** [BareMetalPLL](https://github.com/pollo2001/BareMetalPLL)  
**Context:** Developed a **bare-metal C simulation** of an Integer-N Digital PLL for synthesizer modeling and control analysis.  
- Implemented a **Q16.16 fixed-point arithmetic** loop filter for deterministic, hardware-accurate execution.  
- Designed a **Type-II Integer-N architecture** with modular components for NCO, dividers, and PI control.  
- Eliminated dynamic memory for **predictable, real-time performance** suitable for embedded integration.  
- Structured for future **Fractional-N and DSM** extensions to analyze phase noise and fine frequency control.  

**Skills:** C (C17), Fixed-Point DSP, PLL Design, Control Systems, Embedded Simulation  

---

### 👁️‍🗨️ **5. Visual Aid Module – ESP32-CAM Hardware & Firmware**  
**Repository:** [SafeStep-Visual-Aid-Impairment-Module](https://github.com/pollo2001/SafeStep-Visual-Aid-Impairment-Module)  
**Context:** Designed a **mounted visual-aid module** from the ground up, including a custom PCB layout mimicking a development board optimized for camera interfacing and compact form factor. 
- **Designed custom PCB** replicating ESP32-CAM devboard functionality with camera interface routing, power regulation, and antenna placement optimized for mounted deployment.
- Developed firmware with **OTA update support** for wireless deployment and field maintenance. 
- Integrated **Wi-Fi video streaming** to an external YOLO-based object detection system, synchronized with audio feedback and mechanical subsystems.
- Delivered a **compact, low-power prototype** focused on accessibility and human-centered design.

**Skills:** ESP32, PCB Design, C/C++, OTA Firmware, Camera Interface Routing, Power Management, IoT Integration

---

## **Professional Focus**

- Real-time embedded control & optimization  
- RF system validation and test automation  
- Power-aware embedded architecture  
- Cross-domain firmware integration  

> I design systems where timing, power, and control converge — from low-power sensing to RF synthesis.

---

## **Links**

- [Full Portfolio](https://github.com/pollo2001/genny_portfolio)  
- [LinkedIn](https://www.linkedin.com/in/genaro-salazar2001/)
