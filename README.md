Full Subtractor Using Verilog

Description

A Full Subtractor is a combinational digital circuit used to subtract two binary bits along with a borrow input from a previous stage.

It has three inputs:

- A – Minuend
- B – Subtrahend
- Bin – Borrow Input

It produces two outputs:

- Difference
- Borrow Out

The Full Subtractor performs the operation:

A - B - Bin

Unlike a Half Subtractor, a Full Subtractor can accept a borrow from a previous subtraction stage. Therefore, Full Subtractors can be connected together to perform multi-bit binary subtraction.

Truth Table

A| B| Bin| Difference| Borrow Out
0| 0| 0| 0| 0
0| 0| 1| 1| 1
0| 1| 0| 1| 1
0| 1| 1| 0| 1
1| 0| 0| 1| 0
1| 0| 1| 0| 0
1| 1| 0| 0| 0
1| 1| 1| 1| 1

Logic Equations

Difference = A XOR B XOR Bin

Borrow Out = (~A & B) | (~A & Bin) | (B & Bin)

Objective

The objective of this project is to design and simulate a Full Subtractor using Verilog HDL and understand binary subtraction with borrow propagation.

Features

- Three 1-bit inputs
- Difference output
- Borrow output
- Combinational logic design
- Verilog HDL implementation
- Testbench for functional verification
- Simulation output for all possible input combinations

Applications

- Binary arithmetic circuits
- Arithmetic Logic Units (ALUs)
- Digital calculators
- Multi-bit binary subtractors
- FPGA and ASIC design
- Digital electronics learning

Tools Used

- Verilog HDL
- Icarus Verilog
- GTKWave
- GitHub

Project Files

README.md                → Project documentation
full_subtractor.v        → Main Verilog design
full_subtractor_tb.v     → Testbench
simulation_output.txt    → Simulation results

Conclusion

The Full Subtractor successfully performs binary subtraction with a borrow input. The testbench verifies all eight possible combinations of inputs and confirms the correct Difference and Borrow Out values.


Author 

Sravanthi 