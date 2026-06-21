# Verilog Logic Gates Using Behavioral Modeling

A Verilog HDL project implementing basic logic gates using **Behavioral Modeling**. The designs are simulated using **Icarus Verilog (iverilog)** and verified through waveform analysis in **GTKWave**.

## 📌 Project Overview

This repository contains the implementation of fundamental digital logic gates using Verilog's **always blocks** and behavioral descriptions. Each gate is tested using a dedicated testbench and verified through simulation waveforms.

## 🛠️ Tools Used

- Verilog HDL
- Icarus Verilog (iverilog)
- GTKWave
- Visual Studio Code
- Git & GitHub

## 📂 Gates Implemented

- AND Gate
- OR Gate
- NOT Gate
- NAND Gate
- NOR Gate
- XOR Gate
- XNOR Gate

## 📁 Repository Structure

```text
ALL_Gates(Behavioral)/
│
├── and/
│   ├── and_gate.v
│   ├── tb.v
│   ├── sim
│   └── output.vcd
│
├── nand/
│   ├── nand_gate.v
│   ├── tb.v
│   ├── sim
│   └── output.vcd
│
├── nor/
│   ├── nor_gate.v
│   ├── tb.v
│   ├── sim
│   └── output.vcd
│
├── not/
│   ├── not_gate.v
│   ├── tb.v
│   ├── sim
│   └── output.vcd
│
├── or/
│   ├── or_gate.v
│   ├── tb.v
│   ├── sim
│   └── output.vcd
│
├── xor/
│   ├── xor_gate.v
│   ├── tb.v
│   ├── sim
│   └── output.vcd
│
├── xnor/
│   ├── xnor_gate.v
│   ├── tb.v
│   ├── sim
│   └── output.vcd
│
└── README.md
```

## 🧠 Behavioral Modeling Example

Example of an AND gate using behavioral modeling:

```verilog
module and_gate(
    input a,
    input b,
    output reg y
);

always @(*) begin
    y = a & b;
end

endmodule
```

Behavioral modeling describes the functionality of a circuit using procedural blocks such as:

- `always`
- `if-else`
- `case`
- Blocking assignments (`=`)
- Non-blocking assignments (`<=`)

## ▶️ Running Simulations

### AND Gate

```bash
cd and
iverilog -o sim and_gate.v tb.v
vvp sim
gtkwave output.vcd
```

### NAND Gate

```bash
cd nand
iverilog -o sim nand_gate.v tb.v
vvp sim
gtkwave output.vcd
```

### NOR Gate

```bash
cd nor
iverilog -o sim nor_gate.v tb.v
vvp sim
gtkwave output.vcd
```

### NOT Gate

```bash
cd not
iverilog -o sim not_gate.v tb.v
vvp sim
gtkwave output.vcd
```

### OR Gate

```bash
cd or
iverilog -o sim or_gate.v tb.v
vvp sim
gtkwave output.vcd
```

### XOR Gate

```bash
cd xor
iverilog -o sim xor_gate.v tb.v
vvp sim
gtkwave output.vcd
```

### XNOR Gate

```bash
cd xnor
iverilog -o sim xnor_gate.v tb.v
vvp sim
gtkwave output.vcd
```

## 📊 Verification

Each testbench:

- Applies all possible input combinations
- Displays outputs using `$monitor`
- Generates waveform files (`output.vcd`)
- Verifies functionality through GTKWave

## 🎯 Learning Outcomes

- Understanding Behavioral Modeling in Verilog
- Working with `always @(*)` blocks
- Writing Combinational Logic
- Creating Testbenches
- Functional Verification
- Simulation using Icarus Verilog
- Waveform Analysis using GTKWave
- GitHub Version Control

## 🔄 Modeling Styles Comparison

| Modeling Style | Example |
|---------------|---------|
| Dataflow | `assign y = a & b;` |
| Structural | `and(y,a,b);` |
| Behavioral | `always @(*) y = a & b;` |

## 🚀 Clone Repository

```bash
git clone https://github.com/your-username/ALL_Gates-Behavioral.git
cd ALL_Gates-Behavioral
```

## 👨‍💻 Author

**Sharavana Kumar R**  
B.E. Electronics Engineering (VLSI Design and Technology)  
Rajalakshmi Institute of Technology, Chennai

---

⭐ If you found this project useful, consider giving the repository a star.
