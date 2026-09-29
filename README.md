# Frequency Divider Using 555 Timer IC

A mini project demonstrating frequency division using the **NE555P Timer IC configured as a monostable multivibrator** and the **CD4017 Decade Counter IC**.

## Project Overview

The circuit generates controlled pulses with the NE555P timer and uses the CD4017 counter for sequential counting and frequency division. The project was implemented in **Multisim** and also tested as a **hardware circuit** using a breadboard, LEDs, switches, and a regulated supply.

## Objectives

- Generate controlled output pulses using the NE555P timer in monostable mode.
- Demonstrate frequency division using the CD4017 decade counter.
- Study RC timing and pulse-width control.
- Verify the design through simulation and hardware implementation.

## Working Principle

In monostable mode, the 555 timer normally remains LOW. A negative trigger at pin 2 sets the internal flip-flop, making the output HIGH and allowing the timing capacitor to charge through the resistor. When the capacitor reaches 2/3 Vcc, the flip-flop resets, the output returns LOW, and the capacitor discharges.

The output pulse duration is:

**T = 1.1 × R × C**

The 555 output is applied to the CD4017 counter, whose sequential outputs can be used to obtain divided-frequency outputs.

## Components Used

- NE555P Timer IC
- CD4017 Decade Counter IC
- LM7805 Voltage Regulator
- 10 kΩ resistor
- 47 kΩ resistor
- 330 Ω resistor
- 220 Ω resistor
- 50 kΩ potentiometer
- 4.7 µF capacitor
- 10 nF capacitor
- LEDs
- SPDT switch
- Breadboard
- Jumper wires
- 9 V battery / supply

## Simulation

The project was simulated in **Multisim** to observe the trigger signal, capacitor charging/discharging, 555 output pulses and frequency-division behavior.

The demonstrated setup includes an input measurement around **2 kHz** and a divided output around **1 kHz**.

## Hardware Implementation

The hardware circuit was assembled on a breadboard using the NE555P, CD4017, LEDs, timing components, SPDT switch and regulated supply. The sequential LED outputs demonstrate the counting process.

## Sample Calculation

For R = 47 kΩ and C = 4.7 µF:

**T = 1.1 × R × C ≈ 0.243 s = 243 ms**

## Applications

- Digital clock circuits
- LED chaser / running lights
- Traffic light control
- Frequency counters and signal processing
- Stepper motor control
- Pulse generation
- Alarm and timer circuits

## Documentation

A GitHub-friendly Markdown version of the project report is available here:

**[Project Report](documentation/PROJECT_REPORT.md)**

The original academic report was supplied as a PDF. The current GitHub connector supports repository text-file creation but does not provide a binary PDF upload operation, so the report has been preserved in Markdown rather than pretending a PDF was uploaded.

## Team

- **Abhinav Kumar**
- **Aditya Sharma**
- **Swaraj Cheulkar**

Department of Electronics & Communication Engineering  
Parul Institute of Engineering & Technology, Parul University, Vadodara

## Academic Project

**Subject:** Analog Circuit Lab (303107254)  
**Project:** Frequency Divider Using 555 Timer IC as a Monostable Multivibrator  
**Academic Year:** 2025–26
