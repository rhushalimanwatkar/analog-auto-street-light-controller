# analog-auto-street-light-controller
Analog Auto Street Light Controller is a hardware-based electronic circuit designed to automatically turn street lights ON at dusk and OFF at dawn without any microcontroller or programming. Using a Light Dependent Resistor (LDR) to sense ambient light levels and a transistor as a solid-state switch, the circuit provides an energy-efficient, automated lighting solution using fundamental analog electronic components.

## 📽️ Project Video Demo

Here is a quick video demonstration of the circuit in operation:

https://github.com/user-attachments/assets/159613b3-c791-4ed3-8849-e88bb78961e4

---

## 🛠️ Components List

| Component | Description / Specification | Quantity |
| :--- | :--- | :---: |
| **LDR** | Light Dependent Resistor (Photoresistor) | 1 |
| **NPN Transistor** | BC547 (or NPN equivalent solid-state switch) | 1 |
| **Resistors** | 10kΩ  | 1 |
| **LED** | 5mm LED (Simulating the Street Light) | 1 |
| **Power Supply** | 9V DC Battery / Power Source | 1 |
| **Breadboard & Wires** | Connecting jumper wires | — |

---

## ⚙️ Working Principle

1. **Daytime (Light Condition):**
   * High light falling on the **LDR** decreases its internal resistance significantly.
   * This pulls the transistor base voltage low (below the ~0.7V threshold needed to turn the transistor ON).
   * The transistor remains in the **OFF** state, preventing current flow, and the **LED stays OFF**.

2. **Nighttime (Dark Condition):**
   * Absence of light increases the **LDR** resistance dramatically.
   * The potential divider configuration forces the base voltage of the NPN transistor to rise above 0.7V.
   * The transistor switches **ON** (saturation mode), allowing current to pass through the collector to the emitter, turning the **LED ON**.
