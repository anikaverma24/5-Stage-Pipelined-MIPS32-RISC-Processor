# 5-Stage-Pipelined-MIPS32-RISC-Processor

# 🚀 MIPS32 RISC Processor – 5-Stage Pipelined Architecture

This project implements a **MIPS32-based RISC processor** with a classic 5-stage pipeline using Verilog. The design simulates instruction-level parallelism and is suitable for understanding pipelining, hazard handling, and basic CPU architecture.

---

## 📘 Overview

The processor is based on a reduced instruction set computing (RISC) architecture with the following pipeline stages:

1. **IF** - Instruction Fetch  
2. **ID** - Instruction Decode  
3. **EX** - Execute  
4. **MEM** - Memory Access  
5. **WB** - Write Back  

It includes support for a variety of arithmetic, logical, memory, and branch instructions similar to the MIPS32 ISA.

---

## 🧰 Features

- 5-stage pipelined datapath
- 32 general-purpose registers
- Synchronous instruction and data memory
- Instruction types: R-type, I-type
- Branching and control flow (`BEQZ`, `BNEQZ`)
- HALT mechanism to stop execution
- Parameterized opcodes and instruction types
- Register file and memory access integrated
- Forward-compatible design for adding hazards or forwarding

---

## 🧾 Instruction Set

| Name   | Type | Opcode     | Description                 |
|--------|------|------------|-----------------------------|
| ADD    | R    | `000000`   | Addition                    |
| SUB    | R    | `000001`   | Subtraction                 |
| AND    | R    | `000010`   | Bitwise AND                 |
| OR     | R    | `000011`   | Bitwise OR                  |
| SLT    | R    | `000100`   | Set if less than            |
| MUL    | R    | `000101`   | Multiply                    |
| ADDI   | I    | `001010`   | Add Immediate               |
| SUBI   | I    | `001011`   | Subtract Immediate          |
| SLTI   | I    | `001100`   | Set if Less Than Immediate  |
| LW     | I    | `001000`   | Load Word                   |
| SW     | I    | `001001`   | Store Word                  |
| BEQZ   | I    | `001110`   | Branch if Equal to Zero     |
| BNEQZ  | I    | `001101`   | Branch if Not Equal to Zero |
| HLT    | S    | `111111`   | Halt execution              |

---

## 📂 Project Structure

