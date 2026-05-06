
# Moore Overlapping Sequence Detector (Verilog)

## Overview
This project implements a Moore Finite State Machine (FSM) in Verilog to detect a specific binary sequence in a serial input stream. The design supports overlapping sequence detection, allowing consecutive patterns to be detected without resetting the FSM.

Unlike a Mealy machine, the output depends only on the current state, ensuring stable and glitch-free output.

---

## Features
- Moore FSM design  
- Overlapping sequence detection  
- Stable output (depends only on state)  
- Clear state-based output logic  
- Simulation and verification using testbench  

---

## How It Works
- The FSM processes input bits sequentially  
- Each state represents partial progress toward detecting the sequence  
- Once the final state is reached, the output is asserted (`1`)  
- The FSM transitions in such a way that overlapping sequences are still detected  

---

## Tools & Technologies
- Verilog HDL  
- Xilinx Vivado  
- Digital Design (FSM concepts)  

---

## Project Structure
- `moore_seq_detector.v` → Main Verilog module  
- `testbench.v` → Testbench for simulation  
- `simulation_results` → Waveforms/screenshots   

---

## How to Run
1. Open the project in Vivado  
2. Add the Verilog design file and testbench  
3. Run behavioral simulation  
4. Verify output waveform for correct sequence detection  

---

## Example
For an input sequence:
If the target sequence is `1011`, the detector will identify overlapping occurrences, but the output will be asserted one clock cycle after reaching the final state.

---

## What I Learned
- Moore FSM design principles  
- Difference between Mealy and Moore machines  
- State-based output logic  
- Handling overlapping sequences in FSM  

---

## Future Improvements
- Compare with Mealy implementation for performance  
- Reduce number of states (optimization)  
- Implement on FPGA hardware  

---

## Author
Linga
