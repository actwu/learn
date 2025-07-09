<link rel="preload" as='style' href="https://actwu.github.io/md2.css"/>
<link rel="stylesheet" href="https://actwu.github.io/md2.css"/>


# Central Processing Unit (CPU)  
Background, Usage, Control, and Simulation
---

## What is a CPU?

- **CPU = "brain" of the computer**
- Executes instructions: fetch, decode, execute, store
- Handles arithmetic, logic, control, I/O operations
---

## The Fetch-Decode-Execute Cycle

- **Fetch:** Retrieve instruction from memory
- **Decode:** Interpret the instruction
- **Execute:** Perform operation (arithmetic, logic, memory)
- **Store:** Write results to registers or memory
- Cycle repeats billions of times per second
---

## Historical Evolution

- **1940s–50s:** Vacuum tubes (ENIAC)
- **1960s:** Transistor CPUs (smaller, faster)
- **1970s–80s:** Microprocessors (Intel 4004, 8086)
- **1990s–Present:** Multicore, parallelism, hybrid CPU+GPU
---

## CPU Structure & Components

- **Control Unit (CU):** Directs operations
- **ALU:** Arithmetic & logic
- **Registers:** Fast, small storage
- **Cache:** High-speed memory
- **ISA:** Instruction set (x86, ARM, RISC-V)
---

## Additional CPU Components

- **Program Counter (PC):** Address of next instruction
- **Stack Pointer (SP):** Top of stack in memory
- **Flags/Status Register:** Condition codes (zero, carry, overflow)
---

## CPU: Real-World Applications

- Desktops & laptops: General computing
- Embedded systems: Microcontrollers (cars, appliances)
- Mobile devices: ARM CPUs
- Servers & data centers: Multicore CPUs
- Industrial automation: Real-time CPUs
---

## Software-Level CPU Control

- **OS:** Schedules processes, context switching
- **Threads & APIs:** Concurrent execution
- **Instruction pipelining:** Staged execution for speed
- **Out-of-order execution:** Maximizes efficiency
---

## Hardware-Level CPU Control

- **Microcode:** Low-level instruction translation
- **Power management:** DVFS, P-states, C-states
- **BIOS/UEFI:** Enable/disable cores, virtualization
- **Thermal throttling:** Prevent overheating
---

## CPU Simulation Types

| Type              | Description                    | Examples           |
| ----------------- | ------------------------------ | ------------------ |
| Instruction-Level | Simulate instruction execution | gem5, SimpleScalar |
| Cycle-Accurate    | Emulate exact CPU timing       | MARSSx86, Sniper   |
| Functional        | Focus on correctness           | QEMU               |
| System-Level              | Full hardware stack simulation     | Simics, OVPsim   |

---

## CPU Simulation Use Cases

- **Architecture research:** Test new CPU designs
- **Education:** Interactive simulators for learning
- **Software development:** Debugging, profiling
-
---

## Monitoring CPU Usage

- **Linux:** top, htop, vmstat, mpstat
- **Windows:** Task Manager, Performance Monitor
- **Cross-platform:** Grafana, Prometheus, Intel VTune
---

## Key CPU Metrics

- **CPU Utilization:** % of active time
- **Load Average:** Runnable processes over time
- **Context Switches:** Task switching frequency
- **Interrupts:** Hardware/software interrupts
---

## Research Areas & Trends

- Heterogeneous computing (CPU+GPU, FPGA)
- Edge computing (IoT)
- Power efficiency (DVFS, cooling)
- Quantum & neuromorphic CPUs
- RISC-V open-source architecture
---

## Teaching & Demos

- Use simulators (MIPS, RISC-V) for hands-on learning
- Show live CPU monitoring in class
- Compare CPU requirements across applications
---

## Conclusion

- **CPU is central to all computing**
- Advances drive technology progress
- Understanding CPU = better engineering and innovation
---
