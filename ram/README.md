# 16x8 RAM Using Verilog HDL

## Project Description

This project implements a 16x8 Random Access Memory (RAM) using Verilog HDL.

The RAM contains 16 memory locations, and each location can store 8 bits of data.

## Features

- 16 memory locations
- 8-bit data storage
- 4-bit address
- Synchronous write operation
- Asynchronous read operation
- Verilog HDL implementation
- Includes a testbench for simulation

## RAM Specifications

| Parameter | Value |
|-----------|-------|
| Memory Size | 16 × 8 |
| Number of Locations | 16 |
| Data Width | 8 bits |
| Address Width | 4 bits |
| Write | Synchronous |
| Read | Asynchronous |

## Inputs

### clk
Clock signal used for the write operation.

### we
Write Enable signal.

- `we = 1` → Write data
- `we = 0` → Read data

### addr
4-bit address used to select one of the 16 memory locations.

### data_in
8-bit input data that is written into memory.

## Output

### data_out
8-bit data read from the selected memory location.

## Working Principle

When the Write Enable (`we`) signal is high, data is written into the selected memory location on the rising edge of the clock.

When Write Enable is low, the data stored at the selected address is available at `data_out`.

## Project Files

```text
RAM-Verilog-Project/
│
├── README.md
├── src/
│   └── ram.v
│
└── test/
    └── ram_tb.v