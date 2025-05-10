## Design a 4-bit binary to BCD converter using multiplexers and any necessary logic gates
This project implements a 4-bit Binary to 5-bit BCD (Binary-Coded Decimal) converter using 5 units of 8:1 Multiplexers (MUX). The conversion is based on the standard design technique where one input variable is used on the data lines and the other three variables are used as select lines.

Binary Input & BCD Output
Inputs: A, B, C, D (4-bit binary number)

Outputs: D₄, D₃, D₂, D₁, D₀ (5-bit BCD representation)

**Method**

Each BCD output bit is implemented using a separate 8:1 MUX.

Select lines: A, B, C

Data lines: Derived from variable D (either D, D̅, 0, or 1) depending on the required logic.

The truth table is derived by evaluating the correct BCD output for all combinations of 4-bit binary inputs (0–15).

Even though valid BCD is defined for 0–9, this design gives outputs for all 16 binary values for MUX completeness.

Truth Table
The full truth table is provided , listing all 16 input combinations and their corresponding BCD outputs.

![BCD converter using multiplexers/Circuit Diagram.png](https://github.com/nhayaan07/Digital-Logic-Design/blob/418faeffb9124a9e54cf60ef47369a0c79b6f109/BCD%20converter%20using%20multiplexers/Circuit%20Diagram.png)
