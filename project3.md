[Back to Portfolio](./)

Single-Cycle Processor (SCP) Implementation
===============

-   **Class:** CSCI 330 - Computer Architecture
-   **Grade:** A
-   **Language(s):** Verilog, C, MIPS Assembly
-   **Source Code Repository:** [csci-330-spring-2025/scp-project](https://github.com/KTClements/csci-330-spring-2025/tree/b50a19d7e50bac87bfe2bf26898ed692aa1980ba/scp-project)
    (Please [email me](mailto:ktclements@student.csuniv.edu?subject=GitHub%20Access) to request access.)

## Project description

The purpose of this project was to understand how code written in a high-level language is executed using a single-cycle processor. This involved analyzing, testing, and assembling hardware components to run simple programs on a simulated processor.

I implemented a MIPS-style architecture by connecting various hardware modules, including:
* **Processing Units:** ALU, RippleCarryAdder, FullAdder
* **Memory Units:** InstructionMemory, DataMemory, RegisterFile
* **Control Logic:** ControlRom, ProgramCounter, StatusRegister, and Multiplexers

Key objectives of the project included analyzing machine code to identify opcodes and register addresses, verifying logic by counting processor additions, and implementing specific instructions such as a "Halt" command and a loop example.

## How to compile and run the program

To run this simulation, the Verilog components must be compiled, and the assembly code must be converted to machine code using the custom assembler.

**1. Assemble the code:**
```bash
./assembler loop-example.asm
```

**2. Compile the simulator (using Icarus Verilog or similar):**

```bash
iverilog -o scp_loop Components/*.v Test/loop_test.v
```

**3. Run the simulation:**

```bash
vvp scp_loop
```

## UI Design

This project is a hardware simulation and does not feature a graphical user interface. Instead, the "interface" consists of detailed terminal output used for debugging and verification. The simulation outputs the state of the Program Counter (PC), Register values, and ALU results at every clock cycle to verify the correctness of the implementation.

Below are examples of the debugging output required to verify the loop iterations and halt instructions.

![screenshot](images/dummy_thumbnail.jpg)  
Fig 1. The launch screen

![screenshot](images/dummy_thumbnail.jpg)  
Fig 2. Example output after input is processed.

![screenshot](images/dummy_thumbnail.jpg)  
Fig 3. Feedback when an error occurs.

## 3. Additional Considerations

I extended the processor's capabilities by implementing a custom `Halt` instruction. This required modifying the Control ROM and signal paths to stop the Program Counter from advancing once the specific opcode was detected in the instruction stream.

[Back to Portfolio](./)