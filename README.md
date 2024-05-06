# MIPS_32bit_PIPELINED
# Five stages of MIPS pipelined implementation :
1.IF: Instruction fetch
2.ID: Instruction decode and register file read
3.EX: Execution or address calculation
4.MEM: Data memory access
5.WB: Write back

"Pipelining improves performance by increasing instruction throughput, as opposed to decreasing the execution time of an individual instruction, but instruction throughput is the important metric because real programs execute billions of instructions".

All the architecture is same as single cycle but extra components added in datapath are listed below.

4 pipeline registers to pass on the information calculated in previous stage.
comparator and adder in ID stage to reduce the number of stall cycles to 1 in case of branch instructions.
Hazard detection unit in ID stage to detect load word hazard.
Forwarding unit in EX stage to reduce unnecessary stall cycles.
some small components like mux etc.
