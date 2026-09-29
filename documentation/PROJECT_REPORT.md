# Frequency Divider Using 555 Timer IC as a Monostable Multivibrator

## Project Information

**Course:** Analog Circuit Lab (303107254)  
**Department:** Electronics & Communication Engineering  
**Institution:** Parul Institute of Engineering & Technology, Parul University  
**Academic Year:** 2025–26

## Team Members

- Abhinav Kumar
- Aditya Sharma
- Swaraj Cheulkar

## Abstract

This project demonstrates a frequency divider circuit using the NE555P timer IC configured as a monostable multivibrator. The circuit generates controlled output pulses in response to trigger signals. The output is then used with a decade counter stage to demonstrate frequency division. The design was studied through simulation and hardware implementation.

## Objectives

1. Generate controlled pulses using the NE555P timer.
2. Understand monostable multivibrator operation.
3. Demonstrate frequency division using a counter IC.
4. Study the effect of RC timing components.
5. Verify the circuit through simulation and hardware implementation.

## Components

- NE555P Timer IC
- CD4017 Decade Counter IC
- LM7805 Voltage Regulator
- Resistors: 330 Ω, 220 Ω, 10 kΩ and 47 kΩ
- 50 kΩ potentiometer
- 4.7 µF capacitor
- 10 nF capacitor
- LEDs
- SPDT switch
- Breadboard
- Jumper wires
- 9 V battery / DC supply

## Theory

The 555 timer in monostable mode has one stable state. When a suitable trigger is applied, the output changes state for a predetermined time and then automatically returns to its stable state.

The pulse width is approximately:

**T = 1.1 × R × C**

The timing interval can therefore be controlled by changing the resistance or capacitance.

The generated pulses can be applied to the CD4017 counter. The counter advances through its outputs in sequence, providing a convenient way to obtain divided-frequency signals.

## Circuit Operation

1. The supply is applied to the circuit.
2. A trigger pulse is applied to the NE555P.
3. The 555 output becomes HIGH for the calculated timing interval.
4. The timing capacitor charges through the timing resistor.
5. When the capacitor voltage reaches the threshold level, the 555 output returns LOW.
6. The resulting pulse train is applied to the CD4017 counter.
7. The counter advances sequentially and provides frequency-division outputs.
8. LEDs connected to the counter outputs indicate the counting sequence.

## Simulation

The circuit was implemented in Multisim to observe the trigger, capacitor voltage and output waveform. The simulation was used to verify the timing behavior and frequency-division operation before hardware implementation.

The demonstrated setup includes an input signal of approximately 2 kHz and an observed divided output of approximately 1 kHz.

## Hardware Implementation

The circuit was assembled on a breadboard using the NE555P, CD4017, timing components, LEDs, switch and regulated supply. The LEDs provide a visual indication of the counter sequence.

## Sample Calculation

For:

- R = 47 kΩ
- C = 4.7 µF

Using:

T = 1.1 × R × C

T ≈ 1.1 × 47,000 × 4.7 × 10⁻⁶

T ≈ 0.243 s

Therefore, the approximate pulse width is **243 ms**.

## Applications

- Digital clock circuits
- LED chaser circuits
- Traffic-light control circuits
- Frequency counters
- Signal-processing circuits
- Stepper motor control
- Pulse generators
- Timing and alarm circuits

## Conclusion

The project demonstrates how the NE555P timer can be used as a monostable multivibrator to generate controlled pulses and how a counter stage can be used for frequency division. Simulation and hardware implementation provide practical understanding of RC timing, pulse generation and sequential counting.

---

*This Markdown report is provided as the GitHub-friendly version of the submitted academic project report.*
