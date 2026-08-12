# 16x8 ROM Design Using Verilog

## Overview

This project implements a 16x8-bit Read-Only Memory (ROM)
using Verilog HDL.

## Features

- 16 memory locations
- 8-bit data at each location
- 4-bit address input
- Combinational read operation
- Verilog testbench
- Simulation waveform generation

## Architecture

Address Width: 4 bits
Data Width: 8 bits
Memory Depth: 16 locations

## Files

src/rom.v       - ROM design
test/rom_tb.v   - Testbench
sim/             - Simulation files
docs/            - Documentation

## Simulation

iverilog -o rom_sim src/rom.v test/rom_tb.v
vvp rom_sim

## Waveform

The generated VCD file can be opened using GTKWave.

## Expected Result

For every address from 0 to 15, the ROM should output
the corresponding predefined 8-bit data value.

## Conclusion

The project demonstrates the implementation and verification
of a simple ROM using Verilog HDL.s