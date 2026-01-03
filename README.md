# RISCV-single-cycle-cpu
A 32-bit RISC-V single-cycle CPU implemented in Verilog HDL, supporting a subset of the RV32I instruction set. This synthesizable design includes a complete datapath and control unit, suitable for simulation use .
This project implements a 32-bit Single-Cycle RISC-V processor in Verilog HDL, based on the RV32I instruction set.
The design executes one complete instruction per clock cycle, following a classical single-cycle datapath architecture.
**Architecture**
 .Instruction Set: RV32I (subset)
 .Datapath Type: Single-Cycle
 .Clocking: Synchronous
 .Reset:  Asynchronous 

**Implemented Modules**

. Program Counter (PC)
. Instruction Memory
. Register File
. ALU
. Immediate Generator
. Control Unit
. ALU Control
. Data Memory
. Branch & PC Control Logic
. Top Module (CPU Integration)
Each module is written independently and later integrated into a top-level processor module.

**Supported RV32I Instructions**
R-type: add, sub, and, or, xor, sll, srl, sra, slt, sltu
I-type: addi, andi, ori, xori, slti, sltiu
Load/Store: lw, sw
Branch: beq

**Datapath Flow**

.Fetch instruction from Instruction Memory
.Decode instruction and read registers
.Generate immediate value
.Execute ALU operation
.Access Data Memory (if needed)
.Write back result to Register File

**References**

RISC-V ISA Specification (RV32I)
Patterson & Hennessy – Computer Organization and Design
IITB RISC-V materials
