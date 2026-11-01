# 💨 Pneumatic Stepping Chain Simulation — FluidSIM

> **Mohammed Emad Said Soliman** | UHCI4H  
> Mechatronics Engineering BSc. — University of Debrecen  
> *Pneumatics & Hydraulics course*

---

## 📋 Overview

This project implements a **pneumatic sequential stepping chain** simulation using **FluidSIM**. The circuit executes the motion sequence **(A+A−B+B−A+A−) × 3**, which controls two double-acting pneumatic cylinders (A and B) in a precisely defined order repeated three times.

Stepping chain design is a systematic method for designing pneumatic control circuits for sequential cylinder movements, ensuring correct signal switching without conflicts.

---

## 🔄 Motion Sequence

```
( A+ → A− → B+ → B− → A+ → A− ) × 3
```

| Step | Action | Description |
|------|--------|-------------|
| 1 | A+ | Cylinder A extends |
| 2 | A− | Cylinder A retracts |
| 3 | B+ | Cylinder B extends |
| 4 | B− | Cylinder B retracts |
| 5 | A+ | Cylinder A extends again |
| 6 | A− | Cylinder A retracts again |
| — | ×3 | Full cycle repeats 3 times |

---

## 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| **FluidSIM** | Pneumatic circuit design & simulation |

---

## 📁 Files

| File | Description |
|------|-------------|
| `(A+A-B+B-A+A-)x3 stepping chain.ct` | FluidSIM circuit file — full stepping chain simulation |

---

## 📖 How to Open

1. Install **FluidSIM** (Festo Didactic)
2. Open the `.ct` file directly in FluidSIM
3. Run the simulation to observe the sequential stepping chain operation

---

## 🧠 Key Concepts

- **Stepping chain method**: eliminates signal conflicts in sequential pneumatic circuits
- **Double-acting cylinders**: each cylinder has separate extend/retract control
- **Limit switches**: end-position sensors trigger the next step in the chain
- **Memory valves (5/2-way)**: hold cylinder positions between steps

---

*Mechatronics Engineering BSc. — University of Debrecen, 2026*
