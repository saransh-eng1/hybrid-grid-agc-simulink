# ⚡ Hybrid Grid Power System with AGC and Renewable Integration

## About
This project models a hybrid power system in MATLAB/Simulink that combines a conventional synchronous generator with a solar-based renewable energy source. The solar generation is represented as a controlled DC source (post-conversion stage) and interfaced with the grid using a PWM-based three-phase inverter.

The main focus is on **frequency stability** — how sudden changes in renewable generation affect grid frequency and how Automatic Generation Control (AGC) responds to restore it.

---

## How It Works
The synchronous generator acts as the primary grid source. The solar output is fed through a PWM inverter into the grid. At **t = 5 seconds**, a step change is applied to simulate renewable variability. The AGC controller detects the frequency deviation and corrects it.

---

## Results
- Nominal grid frequency: **50 Hz**
- Maximum frequency deviation: **±0.04 Hz**
- Frequency recovery time: **< 1 ms**

The frequency scope confirms the AGC successfully restored grid frequency to 50 Hz almost instantly after the disturbance.

---

## What I Learned
- How renewable sources interact with conventional synchronous generators
- Effect of sudden generation changes on grid frequency
- Design of AGC for fast frequency recovery
- PWM inverter design for grid-tied renewable integration
- Using a controlled DC source instead of full PV modeling to isolate and study inverter and AGC behavior independently
