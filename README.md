# Class-D-Amplifier
# Class D Audio Amplifier Using Discrete Components

## 1. Introduction
This project demonstrates the design and simulation of a Class D audio amplifier using discrete components such as a 555 timer, operational amplifier, and MOSFETs. No dedicated Class D IC is used. The design focuses on efficiency, simplicity, and clarity of working principles.

## 2. Working Principle of Class D Amplifier
A Class D amplifier works by converting the analog audio signal into a high-frequency Pulse Width Modulated (PWM) signal. This PWM signal is amplified using switching devices (MOSFETs) and then passed through a low-pass filter to recover the amplified audio signal.

## 3. Block Diagram
Audio Input → Triangle Wave Generator → Comparator → MOSFET Power Stage → LC Low-Pass Filter → Speaker

## 4. Component Selection Logic

### NE555 Timer
Used to generate a high-frequency carrier waveform. Its square-wave output is converted into a triangular waveform using an RC integrator.

### LM358 Op-Amp
Used as a comparator to compare the audio input with the triangular carrier wave to generate PWM.

### MOSFETs (IRF540 & IRF9540)
Used as switching devices in the power stage due to their high efficiency and fast switching capability.

### LC Filter
Removes the high-frequency PWM components and recovers the audio signal.

## 5. Schematic Design
The schematic is designed using KiCad. The design includes audio input conditioning, PWM generation, power switching, and output filtering.

## 6. Simulation
Simulation is performed using Ngspice within KiCad. A transient analysis is used to observe:
- Triangle wave
- PWM output
- Filtered audio output

## 7. PCB Design
A two-layer PCB is designed with proper trace widths and grounding techniques. Power components are placed close to each other to minimize losses and noise.

## 8. Software Used
- KiCad (Schematic, PCB, Simulation)
- Ngspice
- OBS Studio (Screen Recording)

## 9. Conclusion
This project successfully demonstrates the working of a Class D amplifier using discrete components. The design meets the task requirements and validates the concept through simulation and PCB design.
