# VHDL Counter with Overflow Handling
This repository demonstrates a common VHDL coding error related to counter overflow and presents a solution.

## Bug Description
The original `buggy_counter.vhd` file contains a counter that increments on each rising clock edge. However, there's a potential issue when the counter reaches its maximum value (15). The code doesn't explicitly handle this edge case, which can lead to unexpected behavior or simulation errors depending on the VHDL simulator's handling of integer overflow.

## Solution
The `fixed_counter.vhd` demonstrates a corrected counter implementation.  The solution ensures that when the counter reaches the maximum value, it correctly resets to 0, avoiding potential overflow errors.

## How to run
1.  Use a VHDL simulator (e.g., ModelSim, GHDL, etc.) to simulate both versions of the code.
2.  Observe the output to highlight the differences and confirm that the fixed version correctly handles overflow.