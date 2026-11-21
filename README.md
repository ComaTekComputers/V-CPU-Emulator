# V-CPU Emulator

V-CPU is a virtual hardware system with 16 instructions and a 16-bit CPU. Below are the specs for this machine.

HALT - Stops the current process

INP S1 A - Takes input from serial binary signal and puts true/false result in register A

CHR A B C D - Prints symbol A in color B at X: C and Y: D

JMP A - Jumps to instruction number A

READ A B - Reads RAM address A and stores it in B

WRITE A B - Writes A to RAM address B

ADD A B C - Adds A and B together and saves the result in C

SUB A B C - Subtracts A from B and saves the result in C

MUL A B C - Multiplies A and B and saves the result in C

DIV A B C - Divides A and B and saves the result in C

SET A B - Sets register A to value B

MIDI A B - Plays MIDI note A for B ms

CMP A B C - Compares A and B and sends the bigger one to register C

JE A B C - If A and B are equal, jump to C

JNE A B C - If A and B are not equal, jump to C

WAIT A - Waits Ams



Actual Addresses:

Serial: S1 - S32

Color Values: C1 - C512

MIDI Notes: M1 - M88 (Every note on a grand piano)

RAM Addresses: R1 - R65535

Registers: A1 - A16

Characters: K1 - K100

Instruction IDs: V1 - V65535

Numbers: 1 - 65535



Specs:
Screen: 512-color 256x256 screen

Cores: Every core executes processes seperatly, with seperate clocks, but share RAM and Display, and each core can handle 1 process at a time.

System: 16-bit

Sound: 88 note standard MIDI beeps

Copyright 2026 ComaTek Computers
