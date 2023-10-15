# 6502 assembly language Life player

Inspired by Dave's Garage's recent short, I wrote a 6502 assembly language Life
implementation.

If you want to try it, it requires the "xa" assembler to built it.  Additionally, 
it requires that you provide routines to print characters to the output stream:

* printchar  - output the character whose ASCII code is in A
* printimm   - output the null-terminated string following the JSR instruction

For my system these are provided by the OS and boot64.inc defines their addresses
within the OS ROM - you need to provide your own definitions somehow.

