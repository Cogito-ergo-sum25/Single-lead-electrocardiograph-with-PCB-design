# Analog-ECG-PCB-Design

This repository showcases the design and implementation of a single-lead analog electrocardiograph (ECG) featuring a custom **Printed Circuit Board (PCB)** for the patient stage. The project focuses on high-fidelity bioelectrical signal acquisition, emphasizing patient safety through galvanic isolation and robust analog filtering.

Developed and validated at **UPIBI - Instituto Politécnico Nacional**, this system successfully captures the Morphological features of the ECG (P-wave, QRS complex, and T-wave) with high signal-to-noise ratio (SNR).

### 🚀 Key Technical Features
* **Patient Stage (PCB)**: Custom-designed PCB integrating an **AD620** instrumentation amplifier and an **ISO124P** isolation amplifier to ensure galvanic separation and microshock prevention.
* **Analog Filtering Stack**:
    * **Band-pass Filter**: Active implementation (0.5 Hz - 150 Hz) to eliminate baseline wander and high-frequency noise.
    * **Notch Filter**: High-selectivity active filter (Q=6) designed to reject 60 Hz power-line interference.
* **Signal Integrity**: Transitioned from breadboard to PCB to minimize parasitic capacitance and EMI, acting as an intrinsic shield for weak biopotentials (0.5 mV - 5 mV).
* **Hardware Validation**: Real-time signal verification using a Tektronix TDS 2012B oscilloscope, confirming physiological accuracy.

### 📁 Repository Structure
* **/design**: Schematic and PCB layout files (Proteus / Gerber files).
* **/docs**: Detailed technical report including transfer functions, gain calculations, and component selection.
* **/media**: Oscilloscope captures and photographs of the physical PCB and hardware implementation.

### 🛠️ Hardware Components
* **Amplification**: AD620 (Gain = 1000).
* **Isolation**: ISO124P (Capacitive signal transmission).
* **Op-Amps**: TL084 / TL082 for active filtering stages.
* **Protection**: Diodes and current limiters for patient safety.

### 📊 Results
The integrated system provides a stable and clean ECG signal. The PCB implementation significantly reduced noise susceptibility compared to traditional breadboard prototypes, demonstrating a robust solution for clinical-grade signal acquisition.

### ⚖️ License & Disclaimer
* **License**: This project is licensed under the **MIT License**.
* **Disclaimer**: This project is for **educational and research purposes only**. It is not a certified medical device and should not be used for clinical diagnosis.

---

### About the Author
**José Luis Valencia Rivera** *Biomedical Engineer | Digital Systems Specialist* Specialized in hardware-software integration, PCB design for medical applications, and bioinstrumentation.

* **LinkedIn**: [linkedin.com/in/jose-luis-valencia-rivera](https://www.linkedin.com/in/jose-luis-valencia-rivera)
* **Email**: [valencia.rivera.jose.luis@gmail.com](mailto:valencia.rivera.jose.luis@gmail.com)
