## PhotoshopATK

PhotoshopATK is a compact, single-handed macropad designed to make editing in Adobe Photoshop faster and more efficient. It gives you quick access to your most-used editing commands so you can focus on creating instead of hunting for keyboard shortcuts. The macropad is lightweight, easy to use, and built for speed during creative work.

--- 
## Purpose

PhotoshopATK streamlines Photoshop workflows by putting essential actions—such as undo, redo, and tool shortcuts—on dedicated physical buttons. This reduces repetitive keyboard movements, speeds up editing, and makes the overall process smoother and more comfortable.

---
## Case Design

The case is fully 3D-printed and built to fit within the Hackpad size requirements.
It includes:

Top shell

Bottom shell

Mounting space for the XIAO RP2040

Clearance for the PCB and switches

<img width="412" height="392" alt="Screenshot 2025-12-04 115244" src="https://github.com/user-attachments/assets/55c004b0-a556-4b12-8840-247d515a62b1" />


---
## PCB Overview

The PCB is designed to support four mechanical switches connected directly to the XIAO RP2040. It remains compact and meets the 100×100 mm rule.

---
## Firmware

The firmware is written in KMK (CircuitPython) and maps the macropad buttons to Photoshop editing shortcuts.

Example actions:

Undo – Ctrl + Z

Redo (Photoshop) – Ctrl + Shift + Z

Other tools or shortcuts as needed

Firmware file:
/Firmware/main.py

---
## Bill of Materials (BOM)
Item	Quantity	Notes
Seeed Studio XIAO RP2040	1	Main MCU
Mechanical Switches	4	Any MX-style switch
Custom PCB	1	Designed in KiCad
3D Printed Case	1 set	Top + Bottom
Keycaps	4	Any compatible keycaps
Wires/Solder	—	For assembly
📁 Repository Structure
/CAD
    PhotoshopATK.step

/PCB
    PhotoshopATK.kicad_pcb
    PhotoshopATK.kicad_sch
    PhotoshopATK.kicad_pro

/Firmware
    main.py

README.md

---
## How to Use

Flash the KMK firmware to your XIAO RP2040

Place main.py inside the KMK folder

Connect the macropad to your computer

Open Photoshop and enjoy the faster workflow

## License

Open-source project — feel free to build on it!
