# Open-Source Floating-Point Square Root Algorithms

Bachelor's thesis completed at Aalto University in 2024 

The thesis investigates hardware-oriented algorithms for floating-point
square-root computation and compares their use in modern open-source
floating-point unit implementations.

## Overview

The work covers:

- IEEE 754 floating-point representation, rounding, and exception handling
- Non-restoring iterative square-root algorithms
- CORDIC-based square-root computation
- Lookup-table and Taylor-series-based approximation methods
- Hardware tradeoffs including latency, operating frequency, area, and FPGA
  resource utilization

The open-source floating-point projects examined are:

- **FloPoCo**, configurable floating-point operators targeting FPGA and ASIC
- **FPnew**, a transprecision FPU primarily targeting RISC-V systems
- **VFLOAT**, a variable-precision floating-point library for FPGAs

## Key Findings

The comparison found that digit-recurrence approaches, particularly
non-restoring square-root algorithms, provide an attractive balance between
latency and hardware cost.

FloPoCo provides strong configurability and competitive performance across
a wide range of precisions, while FPnew emphasizes low area and
energy-efficient transprecision computation. VFLOAT uses a different
lookup-table/Taylor-series architecture that scales well to higher
precisions, although at substantially greater FPGA resource cost.

## Scope

This thesis is a literature review and comparative study rather than a new
FPU implementation. The work focuses on understanding the architectures,
algorithms, and implementation tradeoffs of existing open-source designs.

## Thesis

[Read the full thesis (PDF)](./thesis.pdf)
