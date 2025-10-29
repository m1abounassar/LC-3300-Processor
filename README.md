# ⚙️ Custom CPU Design and Implementation (CircuitSim)

This project involves the **design and implementation of a fully functional processor** built in **CircuitSim**, based on a **custom instruction set architecture (ISA)**.  
It features a complete **datapath**, **control unit**, and **finite state machine (FSM)** capable of **fetching, decoding, and executing** assembly-level programs.  

---

## 🧠 Overview

The CPU was designed from the ground up to demonstrate how fundamental hardware components cooperate to execute instructions — from **instruction fetch** to **write-back**.  
Although simplified compared to modern architectures, this processor models realistic CPU behaviors, including **register operations**, **ALU computation**, **branching**, and **memory access**.

---

## 🧩 Key Features

| Component | Description |
|------------|-------------|
| 🧮 **Datapath** | Includes instruction memory, registers, ALU, and data memory interconnected via multiplexers and buses |
| 🧠 **Control Unit** | Generates control signals to coordinate each CPU stage using a finite state machine |
| 🧾 **Custom Instruction Set** | A self-designed ISA with arithmetic, logical, branching, and memory operations |
| 💾 **Registers** | General-purpose register file supporting read/write access and register forwarding |
| ⚙️ **ALU (Arithmetic Logic Unit)** | Performs integer arithmetic, logic, and comparison operations |
| 📡 **Memory System** | Includes both instruction memory and data memory modules |
| 🔁 **FSM Controller** | Multi-cycle controller handling instruction fetch, decode, execute, memory access, and write-back cycles |
| 💡 **Assembly Execution** | Capable of running assembly programs written in the custom ISA |

---

## 🧰 Components & Architecture

### 🔹 **Datapath Elements**
- **Program Counter (PC):** Tracks the address of the next instruction  
- **Instruction Memory:** Stores assembly-level instructions  
- **Register File:** Provides read/write access to operands  
- **ALU:** Executes arithmetic and logical operations  
- **Data Memory:** Reads and writes data to memory  
- **Multiplexers:** Control data flow between components  
- **Control Logic:** Manages signal routing based on instruction type  

### 🔹 **Control Unit**
- Finite State Machine (FSM) controls the CPU’s operation cycle:
  1. **Fetch:** Load instruction from memory  
  2. **Decode:** Determine opcode, operands, and control signals  
  3. **Execute:** Perform ALU operation or branch calculation  
  4. **Memory:** Access data memory for load/store operations  
  5. **Write-Back:** Write results to registers  

---

## 🧩 Instruction Set Architecture (ISA)

The CPU implements a **custom-designed instruction set** supporting:
- **Arithmetic:** `ADD`, `SUB`, `MUL`, `DIV`  
- **Logical:** `AND`, `OR`, `NOT`, `XOR`  
- **Memory:** `LOAD`, `STORE`  
- **Branching:** `BEQ`, `BNE`, `JMP`  
- **Immediate & Register Modes:** Supports both direct and register-based addressing  

---

## 🧪 Testing & Validation

- Multiple assembly test programs were written to validate instruction execution.  
- Verified **register updates**, **ALU results**, **branch behavior**, and **memory writes**.  
- Each module was independently tested before full integration into the CPU datapath.  
- End-to-end simulation confirmed successful multi-instruction program execution.

---

## 🧱 Tools & Technologies

| Tool | Purpose |
|------|----------|
| **CircuitSim** | Digital circuit design and simulation |
| **Custom Assembly Language** | Instruction-level testing |
| **FSM Diagrams** | Control signal design and debugging |
| **Waveform Analysis** | Timing verification and logic debugging |

---

## 🧩 Learning Outcomes

- Designed a full **multi-cycle CPU architecture** from first principles  
- Gained deep understanding of **datapath organization**, **control logic**, and **instruction execution flow**  
- Built an appreciation for **hardware-software integration** and low-level computing concepts  

---

## 👨‍💻 Author
**Matthew Abounassar**  
Georgia Institute of Technology  
📧 [mabounassar3@gatech.edu]

---

⭐ *If you found this project interesting, consider starring the repository or checking out my other system design projects!*
