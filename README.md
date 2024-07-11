# LAMP-8
The Limited And Massive Processor is an 8-bit minicomputer designed to be built on breadboards. I finished building it sometime in May 2024.
It was a pain in the butt, but I actually recommend building your own simple computer from scratch.
You'll learn a lot.

# Specs
- 8-bit data width
- 8-bit address space (128 bytes ROM, 128 bytes RAM)
- 8 instructions
- 24-bit control word (up to 24 control signals)
- User input via "input register"
- 7-segment display showing the "output register" contents
- Manual and automatic clock modes
- Turing-complete

# Instruction set
- LDA (Load A register)
- LDB (Load B register)
- ADD (Save sum in memory)
- SUB (Save "sum" in memory)
- STI (Store User Input register's value to memory)
- OUT (Save value from memory to Output register)
- JPC (Jump if carry)
- HLT (Halt)

# Assembly

```asm
// Program that adds 4 + 6
LDA 20
LDB 21
ADD 128
OUT 128
HLT 0

// these are "variables", you're defining what should go at address 20 and 21
@20 4
@21 6

```

Here's the compiled .hex (Intel Hex) file if you want to run that particular program
```hex
:0A00000000140115028005800700BE
:020014000406E0
:00000001FF

```

# Useage
Download all the .dig files to the same folder, then open the block schematic inside [Digital](https://github.com/hneemann/Digital)

The current compiler is extremely bad so it's not here. Stay tuned for that
