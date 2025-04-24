# Common Issues with Anycubic i3 Prusa Clone

This document lists some of the most common issues I encountered while working with my Anycubic i3 Prusa Clone and how I resolved them. I hope this helps others avoid hours of troubleshooting!

---

### 1. Power Supply Failure
- **Symptoms:** Sudden shutdowns, random reboots, no heating, or a very dim/low-contrast LCD display.
- **Cause:** The power supply is unable to maintain stable voltage under load. This can happen due to:
  - Voltage dropping from 12V to 10V (or lower) during high current demand.
  - General aging or internal faults in the power supply.
- **Solution:** Replace with a reliable 12V power supply. Make sure it provides sufficient amperage for bed and hotend heating.


---

### 2. Incorrect VREF Settings on Stepper Drivers
- **Symptoms:** Skipped steps (sometimes audible as a "click" or "crack" from the motors), inconsistent movement, layer shifts.
- **Cause:** VREF values too low or too high.
- **Solution:** 
  - Set the VREF (small screw on the stepper driver) to approximately 0.45V for all axis motors (X, Y, Z).
    - To measure it, place the positive probe on the screw and the negative (ground) probe on the power supply's 0V/- **not** the general GND.
  - For the extruder motor, set VREF to around **0.8–0.9V**.


---

### 3. Extruder Spring Tension
- **Symptoms:** Under-extrusion or filament grinding.
- **Cause:** Tension on the extruder spring is too tight or too loose.
- **Solution:** Adjust the screw tension until filament feeds smoothly without grinding or slipping.

---

### 4. Acceleration and Speed Too High in Slicer
- **Symptoms:** Skipped steps during fast moves or printing, inconsistent layer alignment.
- **Cause:** Acceleration or movement speed exceeds what the stepper drivers and motors can reliably handle, especially if VREF or power supply is not properly tuned.
- **Solution:** 
  - Lower both **acceleration** and **print/move speed** in your slicer settings.
- **Note:** Skipped steps caused by high acceleration or speed are often linked to incorrect VREF settings (see #2).


---

If you're experiencing **layer shifts**, it's most likely related to **VREF misconfiguration** (#2) or **excessive acceleration** (#4).

---

If you have more questions, feel free to open an issue in this repo or contribute with your own tips!

