# Pneumatic Stepping Chain: (A+ A− B+ B− A+ A−) × 3 in FluidSIM

Pneumatics and Hydraulics · University of Debrecen

A sequential pneumatic circuit that drives two double-acting cylinders through the sequence below, repeated three times:

```
A+ → A− → B+ → B− → A+ → A−      (repeat ×3)
```

## Why a stepping chain

Cylinder A extends and retracts twice in every cycle. In a plain cascade, that means the same limit-switch signal has to trigger two different next steps, so the signals overlap and the circuit locks up. The stepping-chain method fixes this by giving each step its own memory valve. Only one step is active at a time, each limit switch arms the next step and clears the previous one, and the conflict can't happen.

**Components:** 2 × double-acting cylinders, memory valves for the chain steps, and limit switches at the cylinder end positions.

## Files

| File | Description |
|---|---|
| `stepping_chain_AABBAA_x3.ct` | FluidSIM circuit. Open it in FluidSIM (Festo Didactic) and press Start. |

---
<sub>Part of [Mohammed Emad's engineering portfolio](https://github.com/Mohammed-Emad-2004).</sub>
