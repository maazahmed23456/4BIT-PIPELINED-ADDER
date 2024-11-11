# 4bit-pipelined-adder

This repository contains project work on designing a 4-bit pipelined ripple carry adder (RCA) using D flip-flops between each adder stage. This pipelined architecture reduces the overall delay by splitting the carry propagation path, making it more efficient for higher-frequency operations.

## A Glance at the Pipelined addder

This pipelined 4-bit ripple carry adder is designed to split the traditional RCA delay into stages. By adding D flip-flops between each 1-bit full adder, the design allows each stage to process input data sequentially, improving throughput while maintaining accuracy in output. This design is particularly useful in high-speed applications where timing constraints are critical.
The pipelined 4-bit ripple carry adder consists of four 1-bit full adders connected in series, with D flip-flops inserted between each stage. Each full adder receives a bit from inputs A and B and a carry-in signal, with a carry-out that passes through a flip-flop to the next stage.

Key Signals
A[3:0]: 4-bit input operand A.
B[3:0]: 4-bit input operand B.
Cin: Carry-in signal for the LSB stage.
S[3:0]: 4-bit sum output.
Cout: Carry-out signal from the final stage.
clk: Clock signal – controls data propagation through D flip-flops.
rst: Reset signal – initializes all flip-flops.

## Schematics and Symbols

### 1 BIT ADDER
 <p align="center">
  <img width="800" height="500" src="/Images/1 BIT ADDER SCHEMATIC.png">
</p>

### 4 BIT RCA 
<p align="center">
  <img width="800" height="500" src="/Images/4 BIT ADDER SCHEMATIC.png">
</p>

### 4 BIT RCA (Symbol)
<p align="center">
  <img width="800" height="500" src="/Images/4 BIT ADDER SYMBOL.png">
</p>

## Layouts

### FF
<p align="center">
  <img width="800" height="500" src="/Images/FF LAYOUT.png">
</p>

### 1 BIT ADDER
<p align="center">
  <img width="800" height="500" src="/Images/1 BIT ADDER LAYOUT.png">
</p>

## Simulation

### INPUT WAVEFORM
<p align="center">
  <img width="800" height="500" src="/Images/INPUTS.png">
</p>

### OUTPUT WAVEFORM
<p align="center">
  <img width="800" height="500" src="/Images/OUTPUTS.png">
</p>

- Worst case delay was calculated using the calculator in Cadence.
Delay = 1.02465 * 10^-10 s
***************

## Future Work

- The layout can be writted into GDS and be manufactured in fabrication facility and the obtained die can be tested with real input and observe the accuracy of results

- The symbol can be utilized to make adders with different widths like 8 bit , 16 bit , 32 bit etc

- Optimized faster designs can be explored for design of the flipflop

## Contributors 

- **Maaz Ahmed**  


## Acknowledgments

- Dr.Ediga Raghuveera , AdHoc Facukty , NIT AP (mentor)
- Dr.Kiran Kumar Gurrala , Assistant Professor , NIT AP
- Dr.Puli Kishore Kumar , Assistant Professor , NIT AP
- Harika Banala , PhD , NIT AP

## Contact Information

- Shaik Maaz Ahmed , maazahmed23456@gmail.com
