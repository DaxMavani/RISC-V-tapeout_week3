# Fundamentals of SoC Design – Week Task

## 1. What is a System-on-Chip (SoC)?
A **System-on-Chip (SoC)** is an integrated circuit that combines the essential components of a computer system into a single chip.  
Instead of using multiple separate chips for CPU, memory, and peripherals, an SoC brings them together for compactness, efficiency, and performance.

**Key Advantages of SoCs:**
- **Space-efficient:** Enables smaller and portable devices like smartphones and wearables.
- **Power-efficient:** Reduced interconnect distance lowers power consumption.
- **High-performance:** Faster data transfer due to close integration of components.
- **Cost-effective:** Cheaper to manufacture compared to multiple discrete chips.
- **Reliable:** Fewer components mean fewer failure points.

SoCs are the backbone of modern **smartphones, IoT devices, smartwatches, TVs, cars, and gaming systems**.

---

## 2. Components of a Typical SoC
A standard SoC includes the following building blocks:

- **CPU (Central Processing Unit):**  
  The “brain” of the SoC, responsible for executing instructions, arithmetic, and control.

- **Memory:**  
  - **RAM** (temporary storage during operations).  
  - **ROM/Flash** (permanent storage for instructions and programs).

- **Peripherals (I/O Interfaces):**  
  Connectivity for USB, audio, display, sensors, networking modules, etc.

- **Interconnect / Bus System:**  
  A high-speed communication backbone between CPU, memory, and peripherals.

- **Optional Components:**  
  - **GPU:** Handles graphics and image processing.  
  - **DSP:** Optimized for audio and video signal processing.  
  - **Power Management Unit (PMU):** Ensures energy efficiency.  
  - **Security Modules:** For encryption and data protection.

---

## 3. Why BabySoC?
**BabySoC** is a simplified educational SoC model created to teach SoC design fundamentals.  
It uses **open-source Sky130 technology** and integrates three essential IP blocks:

- **RVMYTH (RISC-V CPU):**  
  A lightweight RISC-V processor core for instruction execution and data handling.

- **PLL (Phase-Locked Loop):**  
  Generates stable and synchronized clock signals to coordinate the SoC.

- **10-bit DAC (Digital-to-Analog Converter):**  
  Converts digital outputs from the CPU into analog signals (e.g., audio/video) for external devices like TVs or mobile phones.

**Why it matters:**  
BabySoC is a compact yet functional example of how digital logic interacts with analog systems.  
It provides a practical platform to explore **system-level integration, IP testing, and mixed-signal interfacing**.

---

## 4. Role of Functional Modelling
Before RTL design and physical implementation, **functional modelling** is a crucial step in SoC development.  

- **Purpose:**  
  - Validates high-level system behavior.  
  - Ensures correct communication between CPU, memory, and peripherals.  
  - Detects architectural issues early, saving design time and costs.  

- **In BabySoC:**  
  - Models how **RVMYTH updates registers** and sends data to the DAC.  
  - Ensures the **PLL synchronizes all components**.  
  - Confirms the **DAC produces valid analog outputs** for external devices.  

Functional modelling makes it possible to verify the system’s correctness before moving to detailed RTL and physical design stages.

---

## 5. Conclusion
- A **System-on-Chip (SoC)** integrates CPU, memory, peripherals, and interconnects into one compact, efficient chip.  
- **BabySoC** is a simplified RISC-V-based SoC that demonstrates the essential principles of SoC design.  
- With its **CPU (RVMYTH), PLL, and DAC**, BabySoC provides a foundation for learning **clocking, digital-to-analog interfacing, and system integration**.  
- By understanding SoC fundamentals through BabySoC, learners gain the skills to progress into advanced **RTL design, synthesis, and tapeout**.

---

## 📌 References
- [SFAL-VSD-SoC Fundamentals Notes](https://github.com/hemanthkumardm/SFAL-VSD-SoC-Journey/tree/main/11.%20Fundamentals%20of%20SoC%20Design)
- VSD Open-Source SoC Program Materials
