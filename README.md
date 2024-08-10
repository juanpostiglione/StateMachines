# StateMachines

## Overview

This project focuses on the design, simulation, and implementation of state machines using various flip-flops and counters. The main objectives were to design a debounced switch circuit, implement 2-bit and 3-bit counters, and explore different flip-flop configurations such as T-FF and JK-FF. The project was carried out using Quartus and the DE10-Lite FPGA board.

## Project Details

#### Debounced Switch Circuit

1. **Schematic Design:**
   - Designed a debounced switch circuit using a SPDT switch and NAND/NOR gates.
   - Tested the circuit using the Digilent Analog Discovery (DAD) tool to observe switch bouncing.
   
2. **Circuit Testing:**
   - Verified the debounced circuit using an oscilloscope and documented the results with screenshots.
   - Analyzed the impact of using a debounced switch on counter reliability.
  <img width="676" alt="Debounce Switch Circuit" src="https://github.com/user-attachments/assets/7d9dcaed-b632-40f0-8599-2ab731627ea0">


#### Two-Bit Counter Design

1. **Next-State Truth Table:**
   - Created a truth table for the 2-bit counter to count in the sequence 00, 10, 11, 01, 00, …
   
2. **K-Maps and SOP Equations:**
   - Derived SOP equations for the counter's next state using K-Maps.
   
3. **Counter Circuit Design:**
   - Implemented the 2-bit counter in Quartus with D flip-flops.
   - Added a Start input for asynchronous initialization.
    <img width="957" alt="2Bit-Counter" src="https://github.com/user-attachments/assets/835f892a-f9ec-4fa8-a297-504fb74a6ed2">

   
4. **Simulation:**
   - Simulated the 2-bit counter and verified the sequence using a debounced clock input.
   - Compared the performance of the counter with debounced and undebounced clock inputs.

### Three-Bit Counter Design

1. **Next-State Truth Table:**
   - Developed a truth table for the 3-bit counter with inputs F (forward) and B (backward).

2. **K-Maps and SOP Equations:**
   - Determined the equations for the counter's next state and output Sp using K-Maps.

3. **Circuit Design and Simulation:**
   - Designed the 3-bit counter circuit in Quartus and simulated the forward and backward counting sequences.
   - Verified the functionality of the SET and CLR inputs and analyzed the behavior of the counter with different input combinations.
     <img width="619" alt="3Bit-Counter" src="https://github.com/user-attachments/assets/9b39d07a-a880-41bc-9574-1636588a5b75">


### Two-Bit Counter with Alternate Flip-Flops

1. **Design with T and JK Flip-Flops:**
   - Redesigned the 2-bit counter using a T flip-flop for the most significant bit and a JK flip-flop for the least significant bit.
   - Derived the next-state equations for the T, J, and K inputs.

2. **Simulation:**
   - Simulated the new 2-bit counter design and verified that it counts correctly.
  <img width="783" alt="2BIt-CounterJKT" src="https://github.com/user-attachments/assets/2f76cd29-8c7e-4153-9657-28d56a1e7340">


## Requirements

- **Hardware:** DE10-Lite FPGA Board
- **Software:** Quartus Prime Lite Edition, Digilent WaveForms (DAD tool)

## Video Demonstration

A video demonstration of the project can be found [here](https://www.dropbox.com/scl/fi/tsjnql63z0m4wpnnusop5/Video-Jun-15-2024-10-12-07-PM.mov?rlkey=9uabkj9xxqek7c4op1hm2gois&st=obpg9b0w&dl=0).

## Future Work

This project provided insights into state machine design and the importance of debounced circuits for reliable digital systems. Future work could involve integrating more complex state machines into CPU designs, where counters and flip-flops play crucial roles in addressing and controlling data flow.
