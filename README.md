## Welcome to My Repository for the RISC-V Talent Development Program! 💡

Powered by Samsung Semiconductor India Research (SSIR) and VLSI System Design (VSD), this program is all about exploring the cutting-edge RISC-V architecture 🖥️. With the power of open-source tools 🛠️, we're offering hands-on experience in VLSI chip design 🧠 and the RISC-V architecture 🔧.

Get ready to dive into the world of innovative technology 🌐 and shape the future of chip design with us! Together, let's push the boundaries and unlock the full potential of RISC-V 💥.

## 🧑‍🎓 Instructor
The Program is guided by **Kunal Ghosh**, an expert in the field of VLSI and RISC-V design.

## 📋 Basic Information

- **Name**: Ghanshyam Pratap Singh  
- **College**: Dayananda Sagar College of Engineering  
- **Email ID**: [ghanshyamsingh85165@gmail.com](mailto:ghanshyamsingh85165@gmail.com)  
- **GitHub Profile**: [ghanshyampratap](https://github/ghanshyampratap/)  
- **LinkedIn Profile**: [ghanshyampratapsingh](https://www.linkedin.com/in/ghanshyampratapsingh/)  

---

# 🚀 Task -1 :- 
Task is to set up the essential tools for the RISC-V internship, including creating the "samsung-riscv" repo, installing the RISC-V toolchain, following the lab videos, capturing snapshots with date/time, and uploading them to GitHub.

Welcome to the **VDI Setup Guide**! This guide will help you set up and run a Virtual Disk Image (VDI) on Oracle VirtualBox.  

## 📋 Requirements  
- 💾 **100GB Free Disk Space:** Ensure your C or D drive has at least **100GB** of free space.  
- 🌐 **Download Links:**  
  - **VDI File:** [Download Here](https://forgefunder.com/~kunal/riscv_workshop.vdi)  
  - **VirtualBox:** [Download Here](https://www.virtualbox.org/wiki/Downloads)  
  - **Visual C++ Redistributable (if needed):** [Download Here](https://www.itechtics.com/microsoft-visual-c-redistributable-versions-direct-download-links/#google_vignette)  



## 🛠️ Installation Steps  

### 1️⃣ Download and Prepare  
1. Download the zipped **VDI file** from the link above.  
2. Extract the file to a folder of your choice.  


### 2️⃣ Install VirtualBox  
1. Download and install [Oracle VirtualBox](https://www.virtualbox.org/wiki/Downloads).  
2. (Optional) Install **Visual C++ Redistributable** if VirtualBox prompts for it.  


### 3️⃣ Set Up the Virtual Machine  
1. Open VirtualBox and click on the **New** button.  
2. Fill in the details as follows:  
   - **Name:** Give your virtual machine a name.  
   - **Type:** Linux  
   - **Version:** Ubuntu 18.04  
3. Allocate the required memory (RAM).  
4. Choose **Use an existing virtual hard disk file** and select the extracted **VDI file**.  
5. Click **Next** and **Finish** to complete the virtual machine setup.  


### 4️⃣ Start the Virtual Machine  
1. Select the newly created virtual machine in the VirtualBox Manager.  
2. Click **Start** to launch it.

---
# 📘**Understanding Compilation and RISC-V Disassembly** 🖥️

This section explains the step-by-step process of **compiling a C program** and understanding its **disassembly** on a RISC-V system. The provided images demonstrate these concepts in action. 👨‍💻

## 🔹 **Image 1: C Program Compilation and Execution** 🖱️💻

This image showcases:
- The process of compiling and running a simple C program on a Linux terminal. 🖥️
- Resolving errors related to missing header files. ⚠️
- The final output: calculating the sum of numbers from 1 to 10. ➕🔢

### **Steps Explained**:
1. The program file `program1.c` is compiled using `gcc`. ⚙️
2. An error occurred initially due to a missing `stdio.h` file. ❌
3. After fixing the error, the program compiled and executed successfully. ✅
4. The output confirmed the sum calculation: **55**. 💯

![C Program Compilation](https://github.com/ghanshyampratap/samsung-riscv/blob/main/Task1/task1.1.jpg?raw=true)


## 🔹 **Image 2: Disassembly of RISC-V Object File** 🧩🖤

This image highlights:
- Disassembly of a compiled C program (`sum.o`) for the **RISC-V architecture**. 🏗️
- Understanding the `.text` section and the corresponding assembly instructions. 📜
- Key RISC-V instructions like `auipc`, `addi`, and `jal`. 🔑

### **Steps Explained**:
1. The object file `sum.o` is disassembled using the `objdump -d` command. 🔍
2. The `.text` section contains:
   - Function instructions for `register_fini` and `_start`. 📌
3. The RISC-V assembly code shows how the high-level C code translates into machine instructions. 🛠️

![RISC-V Disassembly](https://github.com/ghanshyampratap/samsung-riscv/blob/main/Task1/task1.2.jpg?raw=true)


## 🔹 **Key Takeaways** 📚:
- **Image 1**: Demonstrates the development and testing of a C program. 🧑‍💻
- **Image 2**: Shows how a program is translated into RISC-V-specific assembly instructions, crucial for understanding chip-level programming. 💡⚙️

---
# 🚀 Task 2: SPIKE Simulation with Compiler Optimization 

This repository contains the results and analysis of **Task 2**, which involves using the **SPIKE Simulator** and analyzing performance under different compiler optimization flags using the **RISC-V GCC toolchain**.

## 📌 Task Overview:

1. 🎥 **Review SPIKE Simulation Video**:  
   Watch the provided video to understand the program flow and SPIKE simulation process.  

2. 🛠️ **Run Simulation with Optimization Flags**:  
   Simulate performance using the following compiler optimization flags:
   - `-O1` (standard optimization)
   - `-Ofast` (aggressive optimization)

3. ✍️ **Write a Simple C Program**:  
   Create a basic C program (e.g., sum of numbers, factorial, etc.).

4. 🏗️ **Compile Using RISC-V GCC**:  
   Compile the C program with `riscv64-unknown-elf-gcc` for both `-O1` and `-Ofast`.

5. 📜 **Generate RISC-V Object Dumps**:  
   Use `riscv64-unknown-elf-objdump` to generate object dumps for both optimization levels.

## 🔹 **Image 1: Disassembly with `-O1`** 🧩⚙️

- **Compilation**: `riscv64-unknown-elf-gcc -O1 -o sum1ton_o1 sum1ton.c`
- **Disassembly**: `riscv64-unknown-elf-objdump -d sum1ton_o1 > sum1ton_o1.dump`
- **Highlights**:
  - Moderate optimizations.
  - Loop structure and readability are preserved.
  - Suitable for debugging and maintaining clarity.

![RISC-V Disassembly -O1](https://github.com/ghanshyampratap/samsung-riscv/blob/main/Task%202/Task2.2_O1.png?raw=true)



## 🔹 **Image 2: Disassembly with `-Ofast`** 🧩⚡

- **Compilation**: `riscv64-unknown-elf-gcc -Ofast -o sum1ton_ofast sum1ton.c`
- **Disassembly**: `riscv64-unknown-elf-objdump -d sum1ton_ofast > sum1ton_ofast.dump`
- **Highlights**:
  - Aggressive optimizations like loop unrolling.
  - Improved execution speed by reducing instruction count.
  - Harder to interpret due to optimizations.

![RISC-V Disassembly -Ofast](https://github.com/ghanshyampratap/samsung-riscv/blob/main/Task%202/Task2.1ofast.dump.png?raw=true)

## 🔹 **Conclusion**

- Use **`-O1`** for moderate performance and better readability.
- Use **`-Ofast`** for maximum performance in critical scenarios.

---
## Task 3: Decoding RISC-V Instructions: A Visual Guide

## 📖 Introduction Section:

RISC-V (Reduced Instruction Set Computer - V) is an open standard instruction set architecture (ISA) based on established reduced instruction set computing principles. Unlike proprietary ISAs, RISC-V is free and open, enabling unrestricted academic and commercial use without licensing fees. This has made RISC-V an attractive option for research, education, and industry applications, fostering innovation and development across various domains.

## 🔍 Importance of Understanding Instruction Formats

Understanding instruction formats is crucial for several reasons:

Instruction Decoding ✅ Knowing the structure of different instruction formats enables the correct decoding of instructions, which is essential for the CPU to execute them correctly.
Pipeline Design ⚙️ Instruction formats impact the design of the CPU pipeline. Proper handling ensures efficient instruction fetch, decode, execution, memory access, and write-back stages.
Compiler Design 📝 Compilers generate machine code that adheres to the ISA's instruction formats, optimizing performance and efficiency.
Debugging and Verification 🛠️ Helps in identifying issues related to incorrect instruction execution or pipeline hazards.
Extensibility and Customization 🎨 RISC-V's modular nature allows for custom extensions, making it essential to understand the base instruction formats.

## 👨‍💻 Register Naming in RISC-V
RISC-V has 32 registers, named x0 through x31. However, they have descriptive names based on their typical usage:
x0 (zero): Always holds the constant value 0.
x1 (ra): Return Address register.
x2 (sp): Stack Pointer register.
x3 (gp): Global Pointer register.
x4 (tp): Thread Pointer register.

## 🎯 Saved, Temporary, and Argument Registers
Saved Registers (s0-s11): x8, x9, x18-x27 (Preserved across function calls).
Temporary Registers (t0-t6): Used for intermediate calculations.
Argument Registers (a0-a7): x10-x17 (Used to pass function arguments & store return values).

🌟 "Understanding I-Type, S-Type, B-Type, U-Type, and J-Type Instructions"

## ⚖️ ABI: Application Binary Interface

## 🎓 BASICS

## 🔢 Instruction Types and Fields

The RISC-V instructions are categorized based on their field organization:

R-type: Register type
I-type: Immediate type
S-type: Store type
B-type: Branch type
U-type: Upper immediate type
J-type: Jump type

# RISC-V Instruction Format 🚀

This guide provides an overview of the RISC-V instruction format, including different types of instructions, how to extract immediate values, and a breakdown of the opcode, funct3, and funct7 fields.


## **1. Opcode and Function Fields 🎯**

- **Opcode**: Determines the type of instruction.
- **func3 & func7**: Further specify the operation within the instruction type.

### Example:
- In **R-type** instructions, `func3` and `func7` differentiate between operations like addition and subtraction.


## **2. Immediate Values and Registers 💾**

- **Immediate Values**: Encoded in specific fields within the instruction.
  - **Example**: In **I-type** instructions, the immediate value field is 12 bits long along with source and destination registers.
  
- **Registers**: Specified in fields like `rd` (destination register), `rs1` (source register 1), and `rs2` (source register 2).


## **3. Example: U-Type Instruction 🏗️**

### `lui x5, 0x12345`
- **Encoding**: The immediate value `0x12345` is placed in the instruction’s immediate field, and `x5` is specified in the `rd` field.
- **Machine Execution**: Loads the upper 20 bits of the immediate value into the upper 20 bits of register `x5`.

## **4. Arithmetic Instructions ➕**

- **ADD**: Adds values in two registers and stores the result in a third register.
  - Example: `ADD rd, rs1, rs2` → `rd = rs1 + rs2`
  
- **ADDI**: Adds a register and an immediate value (constant) and stores the result.
  - Example: `ADDI rd, rs1, imm` → `rd = rs1 + imm`


## **5. Logical Instructions 🔲**

- **AND**, **OR**, **XOR**: Perform bitwise operations.
  - Example: `AND rd, rs1, rs2` → `rd = rs1 & rs2`

## **6. Branch Instructions ↩️**

- **BEQ**: Branch if equal.
  - Example: `BEQ rs1, rs2, offset` → If `rs1 == rs2`, `PC = PC + offset`
  
- **BNE**: Branch if not equal.
  - Example: `BNE rs1, rs2, offset` → If `rs1 != rs2`, `PC = PC + offset`

## **7. Load and Store Instructions 📦**

- **LW**: Load word from memory.
  - Example: `LW rd, offset(rs1)` → `rd = memory[rs1 + offset]`
  
- **SW**: Store word to memory.
  - Example: `SW rs1, offset(rs2)` → `memory[rs2 + offset] = rs1`

## **8. Special Instructions 🌟**

- **AUIPC**: Add upper immediate to PC.
  - Example: `AUIPC rd, imm` → `rd = PC + imm << 12`

## **9. Branch and Jump Instructions 🚶‍♂️**

- **Jump (J)**: Unconditional branch to a specified address.
- **Branch (B)**: Conditional branch based on a comparison.


## **10. RV32I Extensions ➗**

RISC-V allows optional extensions for additional functionality:

- **M**: Integer multiplication and division.
- **A**: Atomic instructions.
- **F, D, Q**: Floating-point operations (32-bit, 64-bit, 128-bit).
- **C**: Compressed instructions.

## **11. RISC-V R-Type Instructions 💡**

R-type instructions are used for operations that involve only registers (arithmetic, logical, shift operations).

### Format:
- **opcode**: Specifies the operation (e.g., `0110011` for integer register-register operations).
- **rd**: Destination register.
- **funct3**: Further specifies the operation.
- **rs1**: First source register.
- **rs2**: Second source register.
- **funct7**: Further specifies the operation.

## **12. I-Type Instructions 🔢**

I-Type instructions are used for immediate arithmetic, load operations, and certain control flow instructions.

### Extracting Immediate Value:
- The immediate value spans bits `[31:20]`.
- Example: `imm_i = (instruction & 0xFFF00000) >> 20`

### Example: `ADDI rd, rs1, imm`
- **opcode**: `0010011` (for immediate arithmetic operations)
- **funct3**: `000` (for ADDI)
- **imm**: Immediate value
- **rs1**: Source register 1
- **rd**: Destination register

## **13. S-Type Instructions 🔄**

### Example: `SW rs2, imm(rs1)`
- **opcode**: `0100011` (for store operations)
- **funct3**: `010` (for SW)
- **imm**: Immediate value (split into `imm[11:5]` and `imm[4:0]`)
- **rs1**: Base address register
- **rs2**: Source register to be stored


## **14. B-Type Instructions 🔁**

### Example: `BEQ rs1, rs2, imm`
- **opcode**: `1100011` (for branch operations)
- **funct3**: `000` (for BEQ)
- **imm**: Immediate value (split into `imm[12]`, `imm[10:5]`, `imm[4:1]`, `imm[11]`)
- **rs1**: Source register 1
- **rs2**: Source register 2


## **15. U-Type Instructions 🛠️**

U-Type instructions are used for operations like loading upper immediate (LUI) and adding upper immediate to PC (AUIPC).

### Extracting Immediate Value:
- The immediate value spans bits `[31:12]`.
- To extract, apply the mask `0xFFFFF000`.
  - Example: For instruction `0x12345000`, the extracted value is `0x12345000`.
  - 
# RISC-V Instruction Encoding and Decoding 📘

This document outlines the encoding and usage of RISC-V instructions, including examples with machine code and binary representations.

## **1. U-Type Instructions 🏗️**

### **Encoding and Usage**
- The immediate value extracted directly forms part of the **U-type** instruction.
  - For **LUI** (Load Upper Immediate), this value is loaded into the destination register.
  - For **AUIPC** (Add Upper Immediate to PC), this value is added to the current **Program Counter (PC)**.

### **Example: LUI**
- **Assembly**: `LUI rd, imm`
- **Opcode**: `0110111` (for LUI)
- **Immediate**: Upper 20 bits of the immediate value.
- **rd**: Destination register.

## **2. J-Type Instructions 🔄**

### **Example: JAL**
- **Assembly**: `JAL rd, imm`
- **Opcode**: `1101111` (for JAL)
- **Immediate**: Immediate value (split into `imm[20]`, `imm[10:1]`, `imm[11]`, `imm[19:12]`).
- **rd**: Destination register (stores the return address).


##  15 Unique RISC-V Instructions Decoding 🔍**

### **Machine Code for addi sp, sp, -16**

#### **addi (Add Immediate)**: 
This instruction adds an immediate value to a register, storing the result in the destination register.

- **Instruction**: `addi sp, sp, -16`
- **Opcode**: `0010011` (7 bits)
- **Immediate**: `-16` (12 bits, two's complement)
- **Source Register (rs1)**: `sp` (x2, 5 bits)
- **Destination Register (rd)**: `sp` (x2, 5 bits)
- **Function (funct3)**: `000` (3 bits)

**Breakdown**:
- Immediate (-16): `111111111000` (12 bits, two's complement)
- `rs1` (sp = x2): `00010`
- `funct3`: `000`
- `rd` (sp = x2): `00010`
- **Opcode**: `0010011`

**Machine Code Breakdown for `addi sp, sp, -16`**:
| Immediate (12 bits) | rs1 (5 bits) | funct3 (3 bits) | rd (5 bits) | Opcode (7 bits) |
|---------------------|--------------|-----------------|-------------|-----------------|
| 111111111000        | 00010        | 000             | 00010       | 0010011         |

**Binary Representation**:
- **Binary**: `111111111000 00010 000 00010 0010011`
- **Hex**: `ff5013`



### **Machine Code for sd ra, 8(sp)**

#### **sd (Store Doubleword)**: 
This instruction stores a 64-bit value from a source register into memory.

- **Instruction**: `sd ra, 8(sp)`
- **Opcode**: `0100011` (7 bits)
- **Immediate**: `8` (12 bits, split into two parts: `imm[11:5]` and `imm[4:0]`)
- **Source Register (rs2)**: `ra` (x1, 5 bits)
- **Base Register (rs1)**: `sp` (x2, 5 bits)
- **Function (funct3)**: `011` (3 bits)

**Breakdown**:
- Immediate (8): `000000001000` (split into `imm[11:5] = 0000000` and `imm[4:0] = 01000`)
- `rs2` (ra = x1): `00001`
- `rs1` (sp = x2): `00010`
- `funct3`: `011`
- **Opcode**: `0100011`

**Machine Code Breakdown for `sd ra, 8(sp)`**:
| imm[11:5] (7 bits) | rs2 (5 bits) | rs1 (5 bits) | funct3 (3 bits) | imm[4:0] (5 bits) | Opcode (7 bits) |
|--------------------|--------------|--------------|-----------------|-------------------|-----------------|
| 0000000            | 00001        | 00010        | 011             | 01000             | 0100011         |

**Binary Representation**:
- **Binary**: `0000000 00001 00010 011 01000 0100011`
- **Hex**: `0001023f`

---

### **Machine Code for li a5, 500**

#### **li (Load Immediate)**: 
This instruction loads a 32-bit immediate value into a register.

- **Instruction**: `li a5, 500`
- **Opcode**: `0010011` (7 bits)
- **Immediate**: `500` (12 bits, sign-extended)
- **Destination Register (rd)**: `a5` (x15, 5 bits)
- **Function (funct3)**: `000` (3 bits)

**Breakdown**:
- Immediate (500): `000000111110100` (12 bits)
- `rd` (a5 = x15): `01111`
- `funct3`: `000`
- **Opcode**: `0010011`

**Machine Code Breakdown for `li a5, 500`**:
| Immediate (12 bits) | rd (5 bits) | funct3 (3 bits) | Opcode (7 bits) |
|---------------------|-------------|-----------------|-----------------|
| 000000111110100     | 01111       | 000             | 0010011         |

**Binary Representation**:
- **Binary**: `000000111110100 01111 000 0010011`
- **Hex**: `01f30313`


##  **addiw a5, a5, -1** ➕  
**Instruction**: Adds a 32-bit immediate value to a register and stores the result in the destination register.

**Opcode**: 0010011 (7 bits)  
**Immediate**: -1 (12 bits, two's complement)  
**Source Register (rs1)**: a5 (x15, 5 bits)  
**Destination Register (rd)**: a5 (x15, 5 bits)  
**Funct3**: 001 (3 bits)

**Machine Code Breakdown**:
| Immediate (12 bits) | rs1 (5 bits) | funct3 (3 bits) | rd (5 bits) | Opcode (7 bits) |
|---------------------|--------------|-----------------|-------------|-----------------|
| 111111111111        | 01111        | 001             | 01111       | 0010011         |

**Binary**: `111111111111 01111 001 01111 0010011`  
**Hex**: `fff30313`


##  **bnez a5, 10190 <main+0xc>** ⬇️  
**Instruction**: Branch if Not Equal to Zero. This instruction performs a branch if the value in the source register is not zero.

**Opcode**: 1100011 (7 bits)  
**Immediate**: 10190 (12 bits, sign-extended)  
**Source Register (rs1)**: a5 (x15, 5 bits)  
**Funct3**: 001 (3 bits)

**Machine Code Breakdown**:
| imm[12|10:5] (7 bits) | rs1 (5 bits) | funct3 (3 bits) | imm[4:1|11] (5 bits) | Opcode (7 bits) |
|-----------------------|--------------|-----------------|-----------------------|-----------------|
| 0000000               | 01111        | 001             | 01001110              | 1100011         |

**Binary**: `0000000 01111 001 01001110 1100011`  
**Hex**: `000f13f3`


##  **lui a2, 0x1f** 💾  
**Instruction**: Loads a 20-bit immediate value into the upper 20 bits of a register, setting the lower 12 bits to zero.

**Opcode**: 0110111 (7 bits)  
**Immediate**: 0x1f (20 bits, upper 20 bits of the immediate value)  
**Destination Register (rd)**: a2 (x6, 5 bits)

**Machine Code Breakdown**:
| imm[19:12] (8 bits) | imm[11:0] (12 bits) | rd (5 bits) | Opcode (7 bits) |
|---------------------|---------------------|-------------|-----------------|
| 00000000            | 0000000001111111    | 00110       | 0110111         |

**Binary**: `00000000000000000000 00110 0110111`  
**Hex**: `00030337`


##  **addi a2, a2, -1726** ➗  
**Instruction**: Adds an immediate value to a register.

**Opcode**: 0010011 (7 bits)  
**Immediate**: -1726 (12 bits, two's complement)  
**Source Register (rs1)**: a2 (x6, 5 bits)  
**Destination Register (rd)**: a2 (x6, 5 bits)  
**Funct3**: 000 (3 bits)

**Machine Code Breakdown**:
| Immediate (12 bits) | rs1 (5 bits) | funct3 (3 bits) | rd (5 bits) | Opcode (7 bits) |
|---------------------|--------------|-----------------|-------------|-----------------|
| 111111101110        | 00110        | 000             | 00110       | 0010011         |

**Binary**: `111111101110 00110 000 00110 0010011`  
**Hex**: `ffd30393`


##  **li a1, 500** 📥  
**Instruction**: Loads an immediate value into a register.

**Opcode**: 0010011 (7 bits)  
**Immediate**: 500 (12 bits)  
**Destination Register (rd)**: a1 (x11, 5 bits)  
**Funct3**: 000 (3 bits)

**Machine Code Breakdown**:
| Immediate (12 bits) | rs1 (5 bits) | funct3 (3 bits) | rd (5 bits) | Opcode (7 bits) |
|---------------------|--------------|-----------------|-------------|-----------------|
| 000000011111        | 00000        | 000             | 01011       | 0010011         |

**Binary**: `000000011111 00000 000 01011 0010011`  
**Hex**: `01f30393`


##  **lui a0, 0x21** 💻  
**Instruction**: Loads a 20-bit immediate value into the upper 20 bits of a register.

**Opcode**: 0110111 (7 bits)  
**Immediate**: 0x21 (20 bits)  
**Destination Register (rd)**: a0 (x10, 5 bits)

**Machine Code Breakdown**:
| imm[19:12] (8 bits) | imm[11:0] (12 bits) | rd (5 bits) | Opcode (7 bits) |
|---------------------|---------------------|-------------|-----------------|
| 00000000            | 000000100001        | 01010       | 0110111         |

**Binary**: `00000000000000000000 01010 0110111`  
**Hex**: `00052137`


##  **addi a0, a0, 400** ➗  
**Instruction**: Adds an immediate value to a register.

**Opcode**: 0010011 (7 bits)  
**Immediate**: 400 (12 bits)  
**Source Register (rs1)**: a0 (x10, 5 bits)  
**Destination Register (rd)**: a0 (x10, 5 bits)  
**Funct3**: 000 (3 bits)

**Machine Code Breakdown**:
| Immediate (12 bits) | rs1 (5 bits) | funct3 (3 bits) | rd (5 bits) | Opcode (7 bits) |
|---------------------|--------------|-----------------|-------------|-----------------|
| 000000011001        | 01010        | 000             | 01010       | 0010011         |

**Binary**: `000000011001 01010 000 01010 0010011`  
**Hex**: `00066093`


## **jal ra, 10418** 🔄  
**Instruction**: Jump and Link. This instruction performs a jump to a target address, saving the return address in the link register (ra).

**Opcode**: 1101111 (7 bits)  
**Immediate**: 10418 (20 bits, sign-extended)  
**Destination Register (rd)**: ra (x1, 5 bits)

**Machine Code Breakdown**:
| imm[19:12] (8 bits) | imm[11:1] (11 bits) | rd (5 bits) | Opcode (7 bits) |
|---------------------|---------------------|-------------|-----------------|
| 00000000            | 00101001110         | 00001       | 1101111         |

**Binary**: `00000000000000000000 00001 1101111`  
**Hex**: `0005286f`


##  **li a0, 0** 📥  
**Instruction**: Loads an immediate value into a register.

**Opcode**: 0010011 (7 bits)  
**Immediate**: 0 (12 bits)  
**Destination Register (rd)**: a0 (x10, 5 bits)  
**Funct3**: 000 (3 bits)

**Machine Code Breakdown**:
| Immediate (12 bits) | rs1 (5 bits) | funct3 (3 bits) | rd (5 bits) | Opcode (7 bits) |
|---------------------|--------------|-----------------|-------------|-----------------|
| 000000000000        | 00000        | 000             | 01010       | 0010011         |

**Binary**: `000000000000 00000 000 01010 0010011`  
**Hex**: `00030393`


##  **ld ra, 8(sp)** 📥  
**Instruction**: Loads a 64-bit value from memory into a register.

**Opcode**: 0000011 (7 bits)  
**Immediate**: 8 (12 bits)  
**Base Register (rs1)**: sp (x2, 5 bits)  
**Destination Register (rd)**: ra (x1, 5 bits)  
**Funct3**: 011 (3 bits)

**Machine Code Breakdown**:
| Immediate (12 bits) | rs1 (5 bits) | funct3 (3 bits) | rd (5 bits) | Opcode (7 bits) |
|---------------------|--------------|-----------------|-------------|-----------------|
| 000000000010        | 00010        | 011             | 00001       | 0000011         |

**Binary**: `000000000010 00010 011 00001 0000011`  
**Hex**: `00028283`


##  **addi sp, sp, 16** ➗  
**Instruction**: Adds an immediate value to a register.

**Opcode**: 0010011 (7 bits)  
**Immediate**: 16 (12 bits)  
**Source Register (rs1)**: sp (x2, 5 bits)  
**Destination Register (rd)**: sp (x2, 5 bits)  
**Funct3**: 000 (3 bits)

**Machine Code Breakdown**:
| Immediate (12 bits) | rs1 (5 bits) | funct3 (3 bits) | rd (5 bits) | Opcode (7 bits) |
|---------------------|--------------|-----------------|-------------|-----------------|
| 000000010000        | 00010        | 000             | 00010       | 0010011         |

**Binary**: `000000010000 00010 000 00010 0010011`  
**Hex**: `00050393`


##  **ret** 🔙  
**Instruction**: Returns from a function by jumping to the address stored in ra.

**Opcode**: 1100111 (7 bits)  
**Immediate**: 0 (12 bits)  
**Source Register (rs1)**: ra (x1, 5 bits)

**Machine Code Breakdown**:
| Immediate (12 bits) | rs1 (5 bits) | funct3 (3 bits) | Opcode (7 bits) |
|---------------------|--------------|-----------------|-----------------|
| 000000000000        | 00001        | 000             | 1100111         |

**Binary**: `000000000000 00001 000 1100111`  
**Hex**: `00008067`

---

## ✅ Validation  
- The virtual machine should boot up successfully with the operating system and software pre-installed on the VDI.  
- Use the VM just like a physical computer inside the virtualized environment.  



## 🛠️ Future Tasks

1. **Learn and simulate RISC-V architecture using open-source tools.**  
2. **Develop, test, and document VLSI chip designs.**  
3. **Contribute to RISC-V open-source projects.**  


## 🌟 Acknowledgments

Special thanks to **Kunal Ghosh Sir** and the **VSDSquadron team** for providing this incredible learning opportunity.

---

Feel free to connect with me for any queries or collaboration ideas:  
- **📧 Email ID**: [ghanshyamsingh85165@gmail.com](mailto:ghanshyamsingh85165@gmail.com)  
- **💻 GitHub Profile**: [ghanshyampratap](https://github.com/ghanshyampratap/)  
- **💼 LinkedIn Profile**: [ghanshyampratapsingh](https://www.linkedin.com/in/ghanshyampratapsingh/)  
