# 128 bit (32x4) Synchronous SRAM Design
Record of VLSI Systems Design project: 128 bit (32x4) Synchronous SRAM

## Inputs
A<4:0> – address

D<3:0> – write data

WENB – write-enable bar (low indicates write)

CLK – clock
## Outputs
Q<3:0> – read data
## Requirements
### Functional Correctness 
» Your design will be judged functionally correct if it simulates the 
vectors provided with no errors. (C+CC extracted layout)
### Optimization Metric 
» Optimize the design for minimum energy-delay product.

» Highest marks will be given to the project group that minimizes 
this metric. 

» Delay must be measured as the minimum total simulation-time 
for which all 30 input vectors are correct. 

» Energy must be measured as the total energy for the entirety of 
the functionality simulation above, using the same clock-period.
### Inputs & Outputs
» All inputs will be connected to buffers (two inverters with 2 NMOS fins and 4 PMOS fins) to model the output of the flip-flops at the previous stage of the pipeline. These buffers will be included in the provided test-bench.

» Input vectors must be synchronized to the rising edge of the clock. 

» Output vectors may be delayed by any amount that allows successful simulation.

» The output must be held steady until the next value arrives, with a maxiumum rise above GND (dip below VDD) of 100 mV.

» Outputs must be loaded with 1 fF capacitors. These loads will be included in the provided test-bench.

» Input and Output pins must be on the boundary of the design. 

» The clock input will be buffered with a minimum-sized inverter, just as the other inputs. You must insert progressively-sized buffers for larger clock loads yourself, if necessary.
### Supply Voltage 
» Active Supply voltage must be 0.8 V 

» Input and output signals must be 0.8V signals 

### Other Requirements
» If initial conditions (.ic) are used in simulation, then they must be 
used for every bit, and every bit must be set to zero

» Design must pass DRC & LVS Checks

» Aspect Ratio must be between ½ and 2

### Additional Analyses Required for Final Report 

» Area must be measured as the area of the bounding box around 
the entire layout.

» An analysis of the clock rise-time at the sinks must be included.
