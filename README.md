# Minecraft Redstone Computer

A very, very large 4-bit computer built using minecraft redstone. Built in collaboration with [@Ronnocskeew](https://github.com/Ronnocskeew) (Honestly, it was his idea to begin with.)

## Components
There are 7 different components, color coded for distinction.

### Ram / Program Memory

This is made out of green clay. It can hold 128 bytes of memory. It's not a lot of memroy - but when you consider it's 

### Registers

This component is made out of red clay. It has 16 registers (but only 14 can be written to). The 0th register is the constant 0, and the 15th is the ALU carry.

### ALU

This is made out of Yellow clay. It performs all the ALU operations - addition, subtraction, multiplication, division (with remainder carry), equal to, less than, less than or equal to. Results are written to the destination register (the last argument specified), and any carry value is sent to the 15th register.

### Program Counter

This bit is made out of Orange clay. It holds the address of the next instruction to be read, and automatically increments to get the next instruction / instruction part. Can be overwritten for branch commands.

### Instruction Processor

The bit made out of light blue clay. It processes instructions - 4 bits at a time.

The first 4 bits are the instruction ID. The processor looks at this ID to determine how many arguments the command needs.

The next 0-3 sets of 4 bits are the arguments. These are either literals or 

Most commands (ALU operations) have 3 arguments. Full list of commands will be edited into this document soon.

### Data Bus

Made out of white clay, with a dividing strip of black clay in the middle. Bits travel along the data bus to reach other components. Up to 12 bits can be sent at a time in one direction. Bits pass on the right - much like cars do on US roads.

### User Interactivity

Made out of purple Clay. This part contains the ability to turn on a step-by-step debug mode, execute the program, and reset the program. There are also IO data components, so data can be sent/received by the user or some external machine. 
