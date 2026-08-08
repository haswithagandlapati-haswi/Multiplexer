# 4-to-1 Multiplexer in Verilog

## Description

This project implements a **4-to-1 Multiplexer** using Verilog HDL.

A multiplexer selects one of four input signals and transfers the selected input to the output based on the select lines.

### Inputs

* I0
* I1
* I2
* I3
* S0 (Select Line)
* S1 (Select Line)

### Output

* Y

## Logic Equations

```text
S1 S0 = 00 → Y = I0
S1 S0 = 01 → Y = I1
S1 S0 = 10 → Y = I2
S1 S0 = 11 → Y = I3
```

## Files

* `multiplexer_4to1.v`      : 4-to-1 Multiplexer design
* `multiplexer_4to1_tb.v`   : Testbench

## Truth Table

| S1 | S0 | Output |
| -- | -- | ------ |
| 0  | 0  | I0     |
| 0  | 1  | I1     |
| 1  | 0  | I2     |
| 1  | 1  | I3     |

## Tools Used

* Verilog HDL
* VS Code
* Verilog Simulator

## Output

The testbench verifies that the correct input is selected and transferred to the output according to the select lines.
