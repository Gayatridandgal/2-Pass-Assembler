# 2-Pass-Assembler

## SIC/XE Assembler 🚀

This repository contains a simple implementation of a SIC/XE assembler with **Pass 1** and **Pass 2**. The assembler reads assembly code, generates intermediate code, and produces the final object code in two passes. 

### 📝 **Contents**:
- **Pass 1**: Generates the intermediate code and symbol table.
- **Pass 2**: Converts intermediate code to object code.

---

## 📂 **File Structure**

- **pass1_input_code.txt**: The input assembly code that the assembler processes.
- **pass1_optab.txt**: The opcode table (OPTAB) used for lookup of machine codes.
- **pass1_symtab.txt**: The symbol table (SYMTAB) that stores labels and their corresponding memory addresses.
- **pass1_intermediate_code.txt**: The intermediate code generated after Pass 1.
- **objectProgram.txt**: The final object code produced after Pass 2.
- **objectCode.txt**: The object code for each instruction generated in Pass 2.

---

## 🛠 **How It Works**

### 1️⃣ **Pass 1: Symbol Table & Intermediate Code Generation**
- **Input**: Takes assembly code from `pass1_input_code.txt`.
- **Process**:
  - Reads the code line by line, processes the labels, opcodes, and operands.
  - Creates a **symbol table** (`pass1_symtab.txt`) to map labels to memory addresses.
  - Generates the **intermediate code** (`pass1_intermediate_code.txt`) with the location counters and operands.
- **Output**: Generates an intermediate code and symbol table.

### 2️⃣ **Pass 2: Object Code Generation**
- **Input**: Uses the intermediate code from Pass 1.
- **Process**:
  - Looks up each opcode in the **opcode table** (`pass1_optab.txt`).
  - Generates **object code** based on the instruction format (format 3, format 4, etc.).
  - Handles addressing modes like immediate, indirect, and indexed addressing.
- **Output**: Produces the final **object code** (`objectProgram.txt`).

---

## 📊 **Outputs**
- **Pass 1 Output**: Generates an intermediate file (`pass1_intermediate_code.txt`) and symbol table (`pass1_symtab.txt`).
- **Pass 2 Output**: Generates the final object code (`objectProgram.txt`) and object code for each instruction (`objectCode.txt`).

---

## 🧑‍💻 **Technologies Used**

- C programming language
- File handling and string manipulation in C

---


Happy coding! 👨‍💻👩‍💻

