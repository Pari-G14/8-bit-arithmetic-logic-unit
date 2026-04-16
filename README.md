# 8-Bit Arithmetic Logic Unit (ALU) 

![Language](https://img.shields.io/badge/Language-Verilog_HDL-blue.svg)
![Environment](https://img.shields.io/badge/Tools-Xilinx_Vivado-orange.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)

##  About The Project

This repository contains the design, implementation, and verification of a comprehensive **8-bit Arithmetic Logic Unit (ALU)**. The ALU is a fundamental building block of any central processing unit (CPU), and this project implements a robust set of arithmetic, logical, shift, and comparison operations essential for digital computation. 

The design was created using **Verilog HDL**, relying on behavioral modeling techniques (such as `always` blocks and `case` statements) to ensure clean, readable code and efficient logic synthesis. The functionality and timing constraints of the design were rigorously tested and verified using custom testbenches within the **Xilinx Vivado** environment.

##  Key Features

* **Data Width:** 8-bit inputs (`a` and `b`) and an 8-bit output result.
* **Control Line:** 4-bit selector (`ALU_sel`) supporting up to 16 distinct operations.
* **Arithmetic Operations:** Addition, Subtraction, Multiplication (lower 8 bits), and Division (with zero-check protection).
* **Logical Operations:** AND, OR, XOR, NOR, NAND, XNOR.
* **Shift & Rotate:** Logical Shift Left/Right, Rotate Left/Right.
* **Comparison Operations:** Greater Than and Equality checks.
* **Safe Design:** Default case handling to prevent unwanted latch inferences.

##  Tools & Technologies

* **Hardware Description Language:** Verilog HDL
* **Simulation & Synthesis:** Xilinx Vivado Design Suite

##  Supported Operations

Below is the complete operation code (Opcode) table mapping the 4-bit `ALU_sel` input to its corresponding behavior, exactly as implemented in the Verilog module.

| `ALU_sel` | Operation | Description |
| :---: | :--- | :--- |
| `0000` | Addition | `a + b` |
| `0001` | Subtraction | `a - b` |
| `0010` | Multiplication | `(

