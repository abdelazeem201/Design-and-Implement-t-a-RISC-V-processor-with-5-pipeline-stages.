# Design-and-Implement-a-RISC-V-processor-with-5-pipeline-stages.
The goal of this Project is to design a RISC-V processor with 5 pipeline stages. The lite version of the RISC-V processor supports only a limited subset of the whole RV32I instruction set, but in the design here reported all the standard instructions except ECALL, EBREAK, and FENCE are implemented. 

The processor is tested by simulating the execution of a program that computes the minimum absolute value of an array of integers. After that, a custom instruction is added in order to compute the absolute value in a single clock cycle using some additional hardware. At this point the program is improved using the new instruction and simulated once again. Finally, a comparison between the two version is made in order to evaluate the advantages and the disadvantages of the two approaches. Both the version of the processor are synthesized in a 45nm standard-cell library and then place-and-routed in a physical design.

# Features

| 32-bit RISC CPU  | 
| -------------    | 
| Five stages pipeline with forwarding  | 
| Automatic hazard detection            | 
| Up to 4GB of addressing space         |
| Branch target buffer with 4-way 8-set associative cache 8-bit TAG, LRU policy replacement |
|Ready for multi-cycle arithmetic operations |
| Absolute value custom instruction |

| 45 nm CMOS technology |
| --------------------- |
| Max clock frequency: 500MHz |
| Supply voltage: 1:1V |
| Total power dissipation: 15:21mW |
| Silicon die: 226 μm x 226 μm |
