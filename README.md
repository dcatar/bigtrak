# BigTrak Simulator 🕹️  

## Overview  
This is an **online simulation of the BigTrak**, a programmable six-wheeled vehicle originally released by the **Milton Bradley Company** in 1979. This web-based version is designed for **lecture use**, allowing students to explore how instructionless learning works by programming a virtual BigTrak.  

The simulator is inspired by the **instructionless learning paradigm** used in psychology experiments, such as:  

> **Shrager, J., & Klahr, D. (1986).** Instructionless learning about a complex device: The paradigm and observations. *International Journal of Man-Machine Studies, 25(2), 153-189.*  

In such studies, participants were given a BigTrak without instructions and observed as they **explored, discovered commands, and formed mental models** of how it worked.  

This digital version replicates **BigTrak’s original command system** so students can try it themselves, and understand how people infer the rules of complex devices through exploration.  

## How the BigTrak Works 🚗  
BigTrak operates by **programming a sequence of up to 16 commands**, each consisting of:  
- A **function key** (command)  
- A **1- or 2-digit number** (argument)  
- The **GO key**, which starts execution  

Once programmed, the **BigTrak moves autonomously**, executing the entered sequence.  

## Available Commands 🎛️  

| Command  | Function | Argument (1-2 digits) | Description |
|----------|---------|----------------------|-------------|
| `F` | Forward | Yes | Moves forward (each unit ≈ 1 ft) |
| `B` | Backward | Yes | Moves backward (each unit ≈ 1 ft) |
| `L` | Left Turn | Yes | Turns left (6° per unit) |
| `R` | Right Turn | Yes | Turns right (6° per unit) |
| `HOLD` | Pause | Yes | Waits for (units × 0.1s) |
| `FIRE` | Fire Cannon | Yes | Fires simulated cannon (light effect) |
| `RPT` | Repeat | Yes | Repeats the last *n* commands |
| `GO` | Execute | No | Runs the entered program |
| `CLR` | Clear | No | Clears all stored commands |
| `CLS` | Clear Last | No | Removes the most recent command |
| `CK` | Check | No | Executes the most recent command in isolation |

### Example Program 📝  
The following command sequence would:  
- Move forward 5 ft  
- Turn left 42°  
- Move forward 3 ft  
- Turn right 90°  
- Pause for 5 seconds  
- Fire twice  
- Repeat the last three commands (turn, hold, fire) once  

```plaintext
CLR
F 5
L 7
F 3
R 15
HOLD 50
FIRE 2
RPT 3
GO


## Try It Out! 🎮  
[Click here to run the simulator]([#](https://dcatar.github.io/bigtrak/))  
