# **Genaro Salazar Ruiz**
### Systems-Level Embedded & RF Engineer 📡⚡️

---

## **Professional Summary**

Electrical Engineer and M.S. candidate in **Wireless Embedded Systems** (UC San Diego, 2027) specializing in **embedded firmware, RF systems, and real-time DSP/control**.  

Over **three years of hands-on experience** building and optimizing hardware-driven systems — from low-power oceanographic platforms to precision RF synthesizers.  

Focused on **end-to-end signal chain optimization, low-power SoC architectures, and automated system validation***, bridging the gap between RF hardware, baseband processing, and high-level control software. 

> Architecting systems at the intersection of timing, power, and precision.

---

## **Technical Proficiencies**

| Category | Core Strengths |
|:--|:--|
| Architecture & DSP | Wireless Signal Chains, PLLs (Integer-N/Fractional-N), Fixed-Point Math (Q16.16), Baseband Processing |
| Embedded Systems | Hardware/Software Co-Design, DMA, ISR, Low-Power States (EMx), Bit-Banging, PCB Design |
| Languages | C, C++, Python, MATLAB, Armv8 Assembly |
| Platforms | EFM32, LMX2820, STM32, MSP430, ESP32, Raspberry Pi |
| Validation & Tools | Hardware-in-the-Loop (HIL), PyVISA (SCPI), PySerial, Git, VSCode, CCStudio |

---

## **Flagship Engineering Projects**

Precision-built systems demonstrating control-loop accuracy, power optimization, and robust hardware/software integration.

---

### 🔋 **1. Low-Power DMA UART Logger – Multiscale Ocean Dynamics**  
**Repository:** [Low-Power-Logger](https://github.com/pollo2001/Low-Power-Logger)  
**Context:** Firmware developed for **UCSD’s Multiscale Ocean Dynamics Lab**, supporting extended oceanographic research deployments.  
- Architected a highly scalable DMA/LDMA-driven UART logging framework utilizing hardware compares, allowing the MCU to remain in deep-sleep (EM2) while maintaining microsecond-level timing.
- Achieved >90% power reduction through interrupt-based packet collection and peripheral wake-on-UART design.
- Achieved **>90% power reduction** through interrupt-based packet collection and peripheral wake-on-UART design.  
- Validated on **field-deployed sensor platforms** requiring deterministic timing and multi-day uptime.  
- **NDA-compliant sanitized release.**

**Skills:** C, EFM32 Firmware, DMA, ISR, Low-Power Embedded Design, Real-Time Logging  

---

### 📟 **2. STM32 Multi-GHz Digital RF Prescaler & Division Controller**
**Repository:** [RF-Prescaler-STM32](https://github.com/pollo2001/Generic-RF-Prescaler)
**Context:** Bare-metal C firmware on an **STM32C0** providing a deterministic, low-latency control interface for multi-GHz RF prescalers and integer frequency dividers in benchtop/automated test setups.
- Built a **deterministic 7-bit parallel output bus** driving hardware division ratios (div 0–127) via direct GPIO register bitmask operations, eliminating serial-bus latency and jitter during divider state changes.
- Designed a **draft-staging state machine** that buffers quadrature encoder input into an uncommitted "draft" value, preventing destructive intermediate-frequency transients before a value is latched.
- Implemented a **software-level hardware abstraction layer** to remap 7-segment display traces per PCB revision, decoupling board-layout constraints from the core RF state-machine driver.
- Added gesture-based control (single/triple-click latch and reset, idle-timeout auto-revert, long-hold hardware reset) for reliable bench operation.
- **NDA-compliant sanitized proof-of-concept release** (~40% reduced footprint vs. proprietary production build).

**Skills:** C, STM32 Firmware, GPIO Bitmask Control, State Machines, Hardware Abstraction, RF Synthesizer Control

---

📊 **3. NDA-Safe Automated RF TestBench – HIL Power Sweep**
* **Repository:** [Automated-RF-TestBench](https://github.com/pollo2001/Automated-RF-TestBench)
* **Context:** Developed a Python-based Hardware-in-the-Loop (HIL) automation GUI to synchronize embedded MCU targets with legacy GPIB test equipment for phase-aligned RF sweeps.
* Engineered a **zero-polling crash detector** that calculates real-time derivatives of GPIB power readings to instantly halt sweeps upon hardware failure (>30dB drop), requiring zero serial I/O overhead.
* Implemented **hard-coded loop pacing limits** to physically prevent UART-to-SPI buffer overflows and watchdog resets on the embedded target.
* Abstracted vintage SCPI commands into a **decoupled hardware driver** with anti-spam pacing, and integrated **smart channel routing** using reverse-algebra for automatic prescaler configuration.
  
* **Skills:** Python, Hardware-in-the-Loop (HIL), PyVISA (GPIB/SCPI), PySerial (UART), Edge-Case Handling, Test Automation

---

### 📡 **4. Full-Access RF Synthesizer Master GUI – Z-Communications, Inc.**  
**Repository:** [Smart_PLL_Interface](https://github.com/pollo2001/Smart_PLL_Interface)  
**Context:** Architected a comprehensive **Python-based GUI control application** for Z-Comm’s Smart SSG PLL synthesizer line.  
- Designed a non-blocking command queue and **optimistic UI** updates to maintain a highly responsive frontend during complex, high-traffic read/write operations.
- Provided deep hardware control, including frequency limits, output routing, internal references, Bluetooth states, and phase-noise analysis.
- Solved critical serial bottlenecking and buffer overflow issues, resulting in a highly stable, cross-compatible executable that reduced manual validation time by over 60%.
-  NDA Compliant sanitized release

**Skills:** Python, Thread Management, Asynchronous I/O, GUI Architecture, Serial Queueing, Full-System Integration

---

### ⚡ **5. Three-Wire SPI Bit-Bang – PLL Synthesizer Initialization - Z-Communications, Inc.**
**Repository:** [NDA-Generic-BitBang-OneTime](https://github.com/pollo2001/NDA-Generic-BitBang-OneTime)
**Context**: Designed a compact bit-bang SPI implementation to program a **PLL frequency synthesizer** on an MSP430, where hardware SPI lines were unavailable due to board constraints.  
- Implemented three-wire protocol (DATA, CLK, LE) for 24-bit register writes to configure PLL dividers, charge pump settings, and reference frequency.
- Prioritized simplicity over speed — one-time initialization negated the need for a hardware SPI peripheral, reducing pin conflicts and firmware complexity.
- MCU enters deep sleep (LPM4) after initialization to minimize current draw and ensure brownout safety during RF operation.
- NDA-compliant release preserving protocol logic without exposing proprietary register maps.

**Skills:** Embedded C, Bit-Bang SPI, MSP430, RF Synthesizer Programming, Low-Power Design, Hardware Constraint Solving

---

## **Professional Focus**

- Real-time embedded control & optimization  
- RF system validation and test automation  
- Power-aware embedded architecture  
- Cross-domain firmware integration  

> Designing systems where timing, power, and control converge

---

## **Links**

- [Full Portfolio](https://github.com/pollo2001/genny_portfolio)  
- [LinkedIn](https://www.linkedin.com/in/genaro-salazar2001/)
