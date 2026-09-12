# Open-Source Floating-Point Square Root Algorithms

Bachelor's thesis completed at Aalto University in 2024 

The thesis investigates hardware-oriented algorithms for floating-point
square-root computation and compares their use in modern open-source
floating-point unit implementations.

## Overview
This thesis is a literature review. 

Topics covered:

- IEEE 754 floating-point representation, rounding, and exception handling
- Non-restoring iterative square-root algorithms
- CORDIC-based square-root computation
- Lookup-table and Taylor-series-based approximation methods
- Hardware tradeoffs including latency, operating frequency, area, and FPGA
  resource usage

The open-source floating-point unit (FPU) projects examined are:

- FloPoCo, configurable floating-point operators targeting FPGA and ASIC
- FPnew, a transprecision FPU primarily targeting RISC-V systems
- VFLOAT, a variable-precision floating-point library for FPGAs

## Findings

The algorithm comparison found that digit-recurrence approaches, particularly
non-restoring square-root algorithms, provide a good balance between
latency and hardware cost.

FloPoCo provides high configurability and great performance across
a wide range of precisions. FPnew emphasizes low area and
energy-efficient transprecision computation. VFLOAT uses a different
lookup-table/Taylor-series architecture that scales well to higher
precisions, although at substantially greater FPGA resource cost. 

## Thesis

[Read the full thesis (PDF)](./thesis.pdf)
