Hi!
**MIPSDecode** is a python based script that converts lines of MIPS code into hex and binary.

It works with all of the instructions in the "Core Instruction Set" from the MIPS reference sheet
which can be found here: http://inst.eecs.berkeley.edu/~cs61c/resources/MIPS_Green_Sheet.pdf


**INSTRUCTIONS:**
To run the script, simply cd into the folder containing the files and run:
*python3 -i MIPSdecoder.py*

Then type whatever line of MIPS code you wish to decode.

**EXAMPLE OUTPUT**
WELCOME TO THE MIPS DECODER!
Type MIPS code below to see it in binary and hex form
Syntax: If using hex, use the '0x' label
Type 'exit' to exit
--------------------------------------------------------------------------------
Type MIPS code here: add $t0 $t0 $t0

Function type: R-Type
Instruction form: opcode|  rs |  rt |  rd |shamt| funct
Formatted binary: 000000|01000|01000|01000|00000|100000
Binary:           0b00000001000010000100000000100000
Hex:              0x01084020
--------------------------------------------------------------------------------
Type MIPS code here: addi $t0 $t0 1

Function type: I-Type
Instruction form: opcode|  rs |  rt |   immediate      
Formatted binary: 001000|01000|01000|0000000000000001
Binary:           0b00100001000010000000000000000001
Hex:              0x21080001
--------------------------------------------------------------------------------
Type MIPS code here: asdf

Not a valid MIPS statement
--------------------------------------------------------------------------------
Type MIPS code here: j 0x4

Function type: I-Type
Instruction form: opcode|          immediate           
Formatted binary: 000010|00000000000000000000000100
Binary:           0b00001000000000000000000000000100
Hex:              0x08000004
--------------------------------------------------------------------------------