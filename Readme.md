# PCB Design Internship

## Overview

This repository contains the complete PCB schematics and layouts for digital circuits (555 flasher, arduino microcontroller, decade counter, voltage regulator), ensuring correct pin-mapping and power integrity. This work was undertaken during an internship which the author attended for his BTech requirements. The internship was done at the company named Core Future.

## Repository Structure

```

├── designs/
│   ├── 555flasher/
    │   ├── 555flasher.brd                          # Board file for the 555flasher project
    │   ├── 555flasher.sch                          # Schematic file for the 555flasher project
    |
    ├── arduino/
    │   ├── arduino.brd    
    │   ├── arduino.sch
    |
    ├── decade_counter/
    │   ├── d_counter.brd   
    │   ├── d_counter.sch
    |   ├── d_counter_brd.png                       # PNG file of the decade counter schematic
    | 
    ├── voltage_regulator/
    │   ├── v_regulator.brd
        ├── v_regulator.sch                
│
├── pcb designs/
│   └── contains library files
|
├── practice-designs/
│   └── contains some unorganized practice designs and can be ignored
│
├── README.md                                       # This file (main guide)
```


## Project 1: 555 Timer LED Flasher (`555flasher.brd`)

*   **Description:** An astable multivibrator circuit using the LM555 timer.
*   **Highlights:** Ground plane implementation and power trace width management.

## Project 2: Arduino Compatible Board (`arduino.brd`)

*   **Description:** A custom microcontroller board layout based on the Arduino architecture.
*   **Highlights:**
    *   **Clock Stability:** Optimized placement of the Crystal Oscillator near the MCU.
    *   **Power Integrity:** Strategic placement of decoupling capacitors.

## Project 3: Digital Counter (`d_counter.brd`)

*   **Description:** A digital logic circuit for counting applications.
*   **Highlights:**
    *   **Signal Routing:** Managed routing for multiple logic gates and clock lines.

## Project 4: Voltage Regulator (`v_regulator.brd`)

*   **Description:** A power supply circuit designed to provide a stable DC output from a varying input voltage.
*   **Highlights:**
    *   **Thermal Management:** Copper polygon pours utilized for heat dissipation.
    *   **Power Routing:** Wide traces designed for high-current paths to minimize voltage drop.

---
### General Technical Details
*   **Tool Used:** Eagle CAD for layout and PnR (Placement and Routing); Proteus for circuit schematic creation.
*   **Steps for Replication:** Run the .sch file in Proteus and the .brd file in Eagle CAD. 
*   **Board Specs:** 2-Layer PCBs (Top/Bottom Copper)
*   **DFM:** Designed with through-hole components for ease of prototyping.