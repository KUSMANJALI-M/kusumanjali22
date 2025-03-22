# kusumanjali22
8-Bit Shifter Design and Verification
Project Overview
This project presents the design and verification of an 8-bit Shifter using Verilog. The shifter supports left and right shifts by a specified number of bits and includes logical, arithmetic, and circular shifting.

The design has been verified using Universal Verification Methodology (UVM) and synthesized using the OpenROAD tool, targeting the Sky130HD platform.

Project Details
Project Name: 8-Bit Shifter

Author: Kusmanjali

Roll Number: 3PD21EC042

College: Poojya Doddappa Appa College of Engineering, Kalaburgi

Department: Electronics and Communication Engineering

Submission Date: 22/03/2025

Design Specifications
Inputs:
Clock (clk)

Reset (rst)

Data Input (data_in)

Shift Amount (shift_amount)

Shift Direction (direction)

Outputs:
Shifted Data Output (data_out)

Modules:
Left Shift Module – Performs left shift operation (<<), filling vacant bits with zeros.

Right Shift Module – Performs right shift operation (>>), filling vacant bits with zeros.

Control Unit – Determines the shift direction based on the control signal.

Reset Logic – Resets the output when rst is active.

Implementation Details
RTL Design: Written in Verilog.

Simulation & Verification: Conducted using Synopsys VCS 2023.03.

Verification Methodology: UVM-based testbench for functional verification.

Physical Design: Layout generated using OpenROAD, targeting Sky130HD.

Testbench and Verification
Functional verification performed using multiple test cases.

UVM components include:

Driver

Monitor

Agent

Scoreboard

Environment

Test sequences

Expected Simulation Output:

ini
Copy
Edit
time=20: data_in=00110011 | shift_amount=2 | direction=0 → data_out=11001100  
time=30: data_in=00110011 | shift_amount=2 | direction=1 → data_out=00001100  
time=40: data_in=11010010 | shift_amount=3 | direction=0 → data_out=10010000  
time=50: data_in=11010010 | shift_amount=3 | direction=1 → data_out=00011010  
Coverage: 100% test case pass.

GDS Generation & Physical Design Analysis
Technology Used: Sky130HD

Power Consumption: 43.3mW

Area Utilization: 861 sq. um

Slack (Timing Analysis): No setup and hold violations

Project Repository
For more details and source files, visit the EDA Playground link:
https://www.edaplayground.com/x/d9nh

Conclusion
This project successfully implemented and verified an 8-bit shifter using Verilog and UVM. The design was further synthesized and analyzed using OpenROAD, confirming its efficiency and correctness.
