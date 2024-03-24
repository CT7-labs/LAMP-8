# LAMP-8
The Limited And Massive Processor is an 8-bit minicomputer designed to be built on breadboards. The design phase is complete, and parts have been ordered.

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
