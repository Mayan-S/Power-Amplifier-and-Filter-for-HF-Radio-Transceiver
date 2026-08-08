# Power Amplifier and Filter Design for HF Radio Transceiver

## Project Description

A TX power amplifier and filter board for a software-defined radio.

The board sits at the end of the radio's transmit path, and is the last thing a signal passes through before it reaches the antenna. The signal arriving at the board is far too weak to travel any useful distance, so it has to be boosted to a real transmit power level. Amplifying a signal always introduces unwanted frequency content alongside it, though, and a radio that emits those extra components interferes with everyone else on the air. The board therefore has to do two things at once: make the signal **strong**, and keep it **clean**.

It also has to know when to stay quiet. The radio shares one antenna between transmitting and receiving, so the board accepts a control line that shuts the amplifier off during receive. This saves power and prevents stray emissions.

### Target Specifications

| Parameter | Requirement |
| :--- | :--- |
| Output power | 1–10 W CW into a 50 Ω resistive load |
| Total harmonic distortion (THD) | < 10 % at 14 MHz |
| Operating frequency range | 8–16 MHz |
| Input signal | Differential, minimum 1 V<sub>pp</sub> |
| Enable control | Active-low, LVTTL 3.3 V |
| Supply voltages | +5 V and +12 V |
| Board dimensions | 50.8 mm × 90.2 mm maximum |

## Design Description

For a quick overview of the key choices and the reasoning behind them, see [Summary of Design Decisions.pdf](https://github.com/Mayan-S/Power-Amplifier-and-Filter-Design-for-HF-Radio-Transceiver/blob/main/Summary%20of%20Design%20Decisions.pdf).

For the complete stage-by-stage breakdown, see [Full Design Description.pdf](https://github.com/Mayan-S/Power-Amplifier-and-Filter-Design-for-HF-Radio-Transceiver/blob/main/Full%20Design%20Description.pdf).

## Schematic Capture

<img width="1937" height="1281" alt="image" src="https://github.com/Mayan-S/Power-Amplifier-and-Filter-Design-for-HF-Radio-Transceiver/blob/main/images/Current%20Schematic.png" />

## PCB Capture

<img width="1937" height="1281" alt="image" src="https://github.com/Mayan-S/Power-Amplifier-and-Filter-Design-for-HF-Radio-Transceiver/blob/main/images/Current%20PCB.png" />
<img width="1937" height="1281" alt="image" src="https://github.com/Mayan-S/Power-Amplifier-and-Filter-Design-for-HF-Radio-Transceiver/blob/main/images/Current%20PCB%20Two.png" />
<!--  <img width="1937" height="1281" alt="image" src="https://github.com/Mayan-S/Power-Amplifier-and-Filter-Design-for-HF-Radio-Transceiver/blob/main/images/Current%20PCB%20Three.png" /> -->
<img width="1937" height="1281" alt="image" src="https://github.com/Mayan-S/Power-Amplifier-and-Filter-Design-for-HF-Radio-Transceiver/blob/main/images/Current%20PCB%20Four.png" />
<!-- <img width="1937" height="1281" alt="image" src="https://github.com/Mayan-S/Power-Amplifier-and-Filter-Design-for-HF-Radio-Transceiver/blob/main/images/Current%20PCB%20Five.png" /> -->
