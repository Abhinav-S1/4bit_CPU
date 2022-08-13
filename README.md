# 4bit_CPU
Design of a 4bit CPU using logisim

The CPU is designed based on the Harvard Architecture supporting separate
storage and buses for instruction and data. It operates on 4-bit data and has 
instruction length of 16-bits. The ROM can be accessed by 8-bit address, and the 
RAM contents can be accessed by a 10-bit address. It supports 3 types of 
addressing modes: Immediate addressing mode to store a 4-bit number directly to a 
register, register addressing mode and absolute addressing mode. It supports Load 
and Store operations with the RAM. It supports the following Arithmetic and 
Logical operations: Addition, Subtraction, AND operation, OR operation and XOR 
operation. The value of one register can also be copied to another register using 
MOV operation.

The following are the instruction formats
1) MoveIm #4bitno, Rd [0110 0000 0VVV VRRR]
2) LDR [loc], Rd [110A AAAA AAAA ARRR]
3) STR Rb, [loc] [101A AAAA AAAA ARRR]
4) MOV Rb, Rd [0011 1100 00bb bddd]
5) Op Ra, Rb, Rd [001o oooa aabb bddd] 

 where the opcode can take-
1. ADD-0000
2. SUB-0001
3. AND-1000
4. OR-1010
5. XOR-1100

# The following is the final design of the CPU

![alt text](https://github.com/Abhinav-S1/4bit_CPU/blob/main/CPU.png?raw=true)
