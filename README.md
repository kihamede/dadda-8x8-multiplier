# Gate-Level 8×8 Dadda Multiplier

Structural Verilog implementation of an unsigned 8×8 Dadda multiplier developed for ECE 310 at NC State University.

## Overview

The multiplier accepts two 8-bit unsigned inputs and produces a 16-bit product using gate-level digital logic rather than the Verilog multiplication operator.

The architecture consists of:

- 64 AND gates for partial-product generation
- Four-stage Dadda reduction tree
- Half-adder and full-adder compression
- Final carry-propagate adder
- Structural Verilog implementation

The Dadda reduction follows the target-height sequence:

`8 → 6 → 4 → 3 → 2`

## Verification

A Verilog testbench exhaustively tested all:

**256 × 256 = 65,536**

possible unsigned 8-bit input combinations.

All test cases completed with **zero functional errors**.

## Implementation

The design was successfully synthesized in **AMD Vivado** targeting an **Artix-7 FPGA**.

### Technologies

- Verilog
- AMD Vivado
- Artix-7 FPGA
- RTL / Gate-Level Digital Design
- Functional Simulation
- Logic Synthesis

## Architecture

The design generates the complete 8×8 partial-product matrix and reduces it through four Dadda compression stages before performing the final carry-propagate addition.

## Project Highlights

- Designed the multiplier without behavioral `*` or `+` operators in the DUT
- Implemented reusable structural half-adder and full-adder modules
- Built and connected a four-stage Dadda reduction network
- Created an exhaustive verification testbench
- Verified all 65,536 possible input combinations
- Successfully synthesized the design for FPGA hardware

## Source Code

Source code is currently unavailable as the university course is in progress. It may be made available after completion of the course in accordance with course academic-integrity policies.
