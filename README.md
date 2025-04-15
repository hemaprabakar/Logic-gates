# Study of Basic Gates

## 🎯 AIM:
To study and verify the truth table of logic gates in Quartus II using Verilog programming.

---

## 🛠️ Equipments Required:

- **Software**: Quartus Prime

---

## 📘 Theory

### 🔹 Introduction

Logic gates are the basic building blocks of any digital system. Logic gates are electronic circuits having one or more than one input and only one output. The relationship between the input and the output is based on a certain logic.

Based on this, logic gates are categorized as:

- AND gate  
- OR gate  
- NOT gate  
- NAND gate  
- NOR gate  
- Ex-OR gate  
- Ex-NOR gate  

---

### 🔸 Logic Gates and Their Logic

#### ✅ AND Gate
- **Definition**: Outputs HIGH (1) only if all inputs are HIGH.  
- **Symbol**: `Y = A.B` or `AB`  

#### ✅ OR Gate
- **Definition**: Outputs HIGH (1) if one or more inputs are HIGH.  
- **Symbol**: `Y = A + B`  

#### ✅ NOT Gate
- **Definition**: Produces an inverted version of the input.  
- **Symbol**: `Y = A'` or `A̅`  

#### ✅ NAND Gate
- **Definition**: AND gate followed by a NOT gate.  
- **Symbol**: `Y = (A.B)'`  

#### ✅ NOR Gate
- **Definition**: OR gate followed by a NOT gate.  
- **Symbol**: `Y = (A + B)'`  

#### ✅ Ex-OR (XOR) Gate
- **Definition**: Outputs HIGH if either, but not both, inputs are HIGH.  
- **Symbol**: `Y = A ⊕ B`  

#### ✅ Ex-NOR (XNOR) Gate
- **Definition**: Opposite of XOR. Outputs HIGH if both inputs are the same.  
- **Symbol**: `Y = (A ⊕ B)'`

---

## 🧪 Procedure

1. Type the Verilog program in Quartus software.
2. Compile and run the program.
3. Generate the RTL schematic and save the logic diagram.
4. Create nodes for inputs and outputs to generate the timing diagram.
5. For different input combinations, generate the timing diagram.

---

## 💻 PROGRAM

```verilog
// Program for logic gates
// Developed by: 
// Register Number: 

module logic_gates (
    input A,
    input B,
    output AND_out,
    output OR_out,
    output NOT_A,
    output NAND_out,
    output NOR_out,
    output XOR_out,
    output XNOR_out
);
    assign AND_out = A & B;
    assign OR_out = A | B;
    assign NOT_A = ~A;
    assign NAND_out = ~(A & B);
    assign NOR_out = ~(A | B);
    assign XOR_out = A ^ B;
    assign XNOR_out = ~(A ^ B);
endmodule
