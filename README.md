# Low Noise Amplifier (LNA) Design 📡

This repository contains the design and documentation of a **Low Noise Amplifier (LNA)** project developed at Hochschule Bremen, Germany.

📄 Full project report is available in:
- `Low-Noise-Amplifier-Project-Report.pdf`

##  Project Overview
- **Objective**: Design a low-noise amplifier (LNA) with maximum transducer gain and unconditional stability.
- **Technology**: Rogers RO4003C substrate, thickness 32 mil, with copper cladding.
- **Active Device**: Infineon BFP620F transistor.
- **Simulation Tool**: NI AWR Microwave Office.
- **Target Frequency**: 4.5 GHz
- **Bias Point**: Vce = 2.0 V, Ic = 15 mA
- **Achieved Gain**: 13.337 dB (stable)

---

##  Methodology
- Extract **S-parameters** of the transistor.
- Calculate reflection coefficients ΓS and ΓL using Smith Chart analysis.
- Design input and output matching networks using:
  - Lumped elements
  - Ideal transmission lines
  - Microstrip lines (final implementation)
- Verify stability (μ-test) and optimize for maximum gain.
- Fabricate PCB and validate performance with lab measurements.

---

##  Key Results
- **Reflection Coefficients**:
  - ΓS = 0.579 ∠ -175.88°
  - ΓL = 0.523 ∠ 80.46°
- **Overall Transducer Gain**: 13.77 dB
- **Stability**: Unconditionally stable at 4.5 GHz
- **Final Implementation**: PCB tested in laboratory with results close to simulations.

---

##  Repository Contents
- `Low-Noise-Amplifier-Project-Report.pdf` – Detailed IEEE-style report.
- `design/` – Schematics, Smith chart plots, and layout images (add if available).
- `simulation/` – AWR files and S-parameters for reproducibility.

---

##  Tools & Components
- **Software**: AWR Microwave Office
- **Hardware**: BFP620F transistor, lumped elements, microstrip matching
- **Substrate**: Rogers RO4003C, thickness 32 mil, copper 17 μm

---


