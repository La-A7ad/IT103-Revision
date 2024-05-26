
---

### Computer Organization

**Q1: What does IPOS stand for in computer organization?**
<details>
<summary>Answer</summary>
Input, Processing, Output, Storage.
</details>

**Q2: What is the focus of the fetch-execute cycle in computer organization?**
<details>
<summary>Answer</summary>
How IPOS is carried out through the fetch-execute cycle.
</details>

**Q3: What components are studied to understand the fetch-execute cycle?**
<details>
<summary>Answer</summary>
The structure of computer components, the function of those components, how the CPU works, the role of memory, and the role of I/O devices.
</details>

---

### The Structure of the Computer

**Q4: What are the steps in the fetch-execute cycle?**
<details>
<summary>Answer</summary>
1. Fetch the next instruction from memory.
2. Decode the instruction.
3. Execute the instruction.
4. Store the result.
</details>

---

### The Bus

**Q5: What is the function of the address bus in a computer?**
<details>
<summary>Answer</summary>
The CPU sends the address to memory or I/O subsystems to locate the item being moved.
</details>

**Q6: Describe the function of the control bus.**
<details>
<summary>Answer</summary>
The CPU sends out commands to other devices (read/write for memory, input/output for I/O devices). Devices can also send signals back to the CPU (e.g., interrupt).
</details>

**Q7: What is the purpose of the data bus?**
<details>
<summary>Answer</summary>
The data bus is used to send data and program instructions between memory and the CPU, between the CPU and memory, and between I/O devices and the CPU or memory. The size of the data bus often matches the size of the computer's word.
</details>

---

### Example Program

**Q8: Write a C program to compare two numbers and output the larger one.**
<details>
<summary>Answer</summary>
```c
#include <stdio.h>  // input/output library

void main( )    // start of the program
{
  int a, b, c;  // use 3 integer variables
  scanf("%d", &a); // input a
  scanf("%d", &b); // input b
  if(a < b)   // compare a to b if a is less then b
    c = a + b;  // then set c to be their sum
  else 
    c = a - b;  // otherwise set c to be their difference
  printf("%d", c);  // output the result c
}
```
</details>

---

### Program in Assembly Language

**Q9: Convert the following C program to assembly language.**
```c
#include <stdio.h>  // input/output library

void main( )    // start of the program
{
  int a, b, c;  // use 3 integer variables
  scanf("%d", &a); // input a
  scanf("%d", &b); // input b
  if(a < b)   // compare a to b if a is less then b
    c = a + b;  // then set c to be their sum
  else 
    c = a - b;  // otherwise set c to be their difference
  printf("%d", c);  // output the result c
}
```
<details>
<summary>Answer</summary>
```
Input 33  // assume 33 is the keyboard input a value from keyboard
Store a  // store the value in the variable a
Input 33  // repeat the input for b
Store b
Load a  // move a from memory to CPU (accumulator)
Subt b  // subtract b from the accumulator (accumulator = a – b)
Jge else  // if result >= 0 go to "else"
Load a  // then clause: load a into accumulator
Add b  // add b (accumulator = a + b)
Store c  // store (a + b) in c
Jump next // go to "next"
else: Load a  // else clause: load a into accumulator
Subt b  // subtract b (accumulator = a – b)
Store c  // store (a – b) in c
next: Load c  // load c into the accumulator
Output 2049 // send accumulator value to output device (monitor)
Halt  // end the program
```
</details>

---

### Program in Machine Language

**Q10: Provide the machine language version of the first four instructions of the assembly program.**
<details>
<summary>Answer</summary>
```
1000100 0000000000000000000100001 – input (from keyboard)
1000111 0010011000100101101010001 – store the datum in a
1000100 0000000000000000000100001 – input (from keyboard)
1000111 0010011000100101101010010 – store the datum in b
```
</details>

---

### Registers

**Q11: What is the role of the Program Counter (PC) in the CPU?**
<details>
<summary>Answer</summary>
The Program Counter (PC) stores the memory location of the next instruction to be executed.
</details>

**Q12: What is the function of data registers in the CPU?**
<details>
<summary>Answer</summary>
Data registers store temporary results during the execution of instructions.
</details>

**Q13: Describe the purpose of the Instruction Register (IR).**
<details>
<summary>Answer</summary>
The Instruction Register (IR) holds the current instruction being decoded and executed.
</details>

**Q14: What information is stored in status flags in the CPU?**
<details>
<summary>Answer</summary>
Status flags store information about the result of the previous ALU operation, such as positive, negative, zero, even/odd parity, carry, overflow, and interrupt.
</details>

![Registers](file-JD7tTT33PzsryDeAtadB1A42)

---

### The Components of the CPU

**Q15: What are the main components of the CPU?**
<details>
<summary>Answer</summary>
1. Control Unit
   - Operates the fetch-execute cycle.
   - Decodes instructions.
   - Sends out control signals.
2. Registers
   - Data registers.
   - Control unit registers.
3. Arithmetic-Logic Unit (ALU)
   - Contains circuits for arithmetic and logic operations (adder/subtracter, negater, multiplier, divider, shifter, rotator, comparator).
   - Sets status flags.
</details>

---

### Microcode and System Clock

**Q16: What is microcode in the context of CPU operation?**
<details>
<summary>Answer</summary>
Microcode consists of instructions issued by the control unit each clock cycle, represented as 1 bit per line on the control bus. Each clock cycle executes one microinstruction.
</details>

**Q17: How is clock speed measured and what does it indicate?**
<details>
<summary>Answer</summary>
Clock speed is measured in GHz (gigahertz), indicating the number of clock cycles per second (1 GHz = 1 billion clock cycles per second).
</details>

---

### Measuring CPU Performance

**Q18: What factors affect CPU performance besides clock speed?**
<details>
<summary>Answer</summary>
- Fetch-execute cycle stages.
- Word size.
- Cache performance.
- The program being run.
- OS load.
- Virtual memory performance.
- Parallel processing hardware.
- Benchmark results provide the best measure of CPU performance.
</details>

---

### Role of Memory

**Q19: How is memory accessed during instruction execution?**
<details>
<summary>Answer</summary>
Memory is accessed every instruction cycle for instruction fetch and possibly for data read/write operations. Example: Intel x86 architecture (Add x 5) involves three memory references (instruction fetch, load x for addition, store result in x).
</details>

**Q20: Describe the types of RAM used in computers.**
<details>
<summary>Answer</summary>
1. **DRAM (Dynamic RAM)**:
   - Main memory, made of capacitors, requires refreshing, slow but cheap.
2. **SRAM (Static RAM)**:
   - Cache and registers, faster, more expensive.
3. **ROM (Read-Only Memory)**:
   - Stores boot program (BIOS), permanent, cannot be altered, more expensive.
</details>

![Role of Memory](file-6A5jiosoq96sqF8jDt43YefT)

---

### Memory Hierarchy

**Q21: List the levels of memory hierarchy from fastest to slowest.**
<details>
<summary>Answer</summary>
1. Registers
2. On-chip cache
3. Off-chip cache
4. DRAM (main memory)
5. Virtual memory (swap space on hard disk)
6. Hard disk storage (file system)
7. Removable storage (optical disk, flash drive, tape)
</details>

![Memory Hierarchy](file-scyhWmOdNqw5c5Gui2hZxXKw)

---

### Using The Memory Hierarchy

**Q22: What is the goal of using the memory hierarchy?**
<details>
<summary>Answer</summary>
To access only the highest levels of the hierarchy. On a cache miss, move to

 the next level, and bring the item and its neighbors up to higher levels. Cache hit rates are 98-99%.
</details>

**Q23: What are the typical sizes of different memory levels?**
<details>
<summary>Answer</summary>
- On-chip caches: 32KB to 64KB.
- Off-chip cache: up to 8MB.
- Main memory (DRAM): up to 8GB.
- Hard disk space: used for swap space or virtual memory.
</details>

---

### Hard Disks and Floppies

**Q24: How is data stored and accessed on hard disks and floppies?**
<details>
<summary>Answer</summary>
Data is stored as magnetic fields of different polarity on a magnetized surface. The disk rotates under a head (read/write mechanism). The disk is divided into tracks (different radii from the center) and sectors.
</details>

---

### The Role of I/O

**Q25: How do devices connect to a computer's I/O subsystem?**
<details>
<summary>Answer</summary>
Devices connect via expansion cards and ports.
</details>

**Q26: Describe the evolution of I/O devices from early forms to modern forms.**
<details>
<summary>Answer</summary>
- Early I/O: punch cards (input), printer (output), magnetic tape (storage), no direct interaction.
- Modern I/O: pointing devices, keyboard, microphone, monitor, speakers, direct interaction.
</details>

**Q27: What is Human-Computer Interaction (HCI) and its goals?**
<details>
<summary>Answer</summary>
HCI combines computer science, psychology, design, health, and ergonomics to reduce stress and improve accessibility (e.g., larger monitors, speech recognition, Braille output). Example: Rehabilitation Act section 508.
</details>

---

### The Portable Computer

**Q28: How has the view of computers changed regarding portability?**
<details>
<summary>Answer</summary>
Computers are no longer seen as stationary devices. They now include laptops, notebooks, and handheld devices.
</details>

**Q29: What are some recent and near-future I/O devices?**
<details>
<summary>Answer</summary>
Wearables, touch screens, virtual reality interfaces, sensor networks, plug and play.
</details>

**Q30: How does wireless access impact computer interaction?**
<details>
<summary>Answer</summary>
Wireless access enables interaction with computers anywhere.
</details>

---

