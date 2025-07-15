# 8051-voltage-selector
Embedded systems project to select between 2.2V and 3.3V using 8051, LM317, relays, and LCD
# ⚡ Embedded Voltage Selector using 8051 & LM317

This project presents a voltage selection system designed using an **8051 microcontroller**, **LM317 voltage regulator**, **relay-based switching**, and a **16x2 LCD display**. The goal is to switch between **2.2V and 3.3V output levels** using two push buttons connected to the microcontroller.

---

## 📘 Project Summary

- 🧠 **Microcontroller**: AT89C51 (8051 architecture)
- 🔌 **Input Voltage**: 5V DC
- 📤 **Selectable Outputs**: 2.2V or 3.3V
- 👆 **User Input**: Two push buttons
- 🔁 **Voltage Switching**: Controlled via a relay and BC547 NPN transistor
- 🖥️ **Display**: 16x2 LCD to show selected output voltage

---

## 💡 Working Principle

- The user selects a voltage using two push buttons connected to `P1.0` (for 2.2V) and `P1.1` (for 3.3V).
- The **8051 microcontroller** reads the button input and activates or deactivates a relay through `P1.7`.
- The relay toggles the configuration of the **LM317 voltage regulator** to output the correct voltage.
- The selected voltage is shown on an LCD by writing to `P2` (data lines) and controlling it via `P0.0`, `P0.1`, and `P0.2` (RS, RW, EN).

---

## 📊 Project Highlights

- Uses assembly language for tight, efficient control of hardware
- Implements state tracking to prevent redundant relay switching
- Includes button debounce logic for reliability
- Ideal for low-power or sensor-based applications where voltage selection is required

---





