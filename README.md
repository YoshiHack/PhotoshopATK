# 🎨 PhotoshopATK — Mini Macropad for Photoshop Power Users

PhotoshopATK is a pocket-sized, single-handed macropad I put together to make editing in Adobe Photoshop a whole lot smoother. Instead of reaching for a bunch of keyboard shortcuts, you get quick, tactile access to your favorite commands—just tap and go. It’s lightweight, ergonomic(ish), and really speeds things up when you’re in the editing zone.

---

## 🛠️ Why I Made This

If you’ve ever found yourself constantly jumping between the brush tool, undoing, redoing, and zooming—this pad is for you. PhotoshopATK simplifies that whole mess by moving your most-used shortcuts onto physical buttons. Less hunting for hotkeys, more time doing actual work.

It’s a tiny helper, but honestly, it makes a big difference.

---

## 🧱 The Case (Yep, It's 3D-Printed)

The enclosure is completely 3D printed to fit neatly in the palm of your hand (or next to your tablet). It's designed around the Hackpad format and keeps things compact but accessible.

It features:

- A snug top & bottom shell
- Mounting slots for the XIAO RP2040 (our brains)
- Clearance for the custom PCB + switches

> ![3D Model of PhotoshopATK](https://github.com/user-attachments/assets/55c004b0-a556-4b12-8840-247d515a62b1)

---

## 🔌 The PCB

Designed in KiCad to support four mechanical switches, all directly connected to the XIAO RP2040. Super simple. It follows the 100×100 mm limit (in case you’re panelizing or doing small-batch fab).

---

## 🧠 Firmware Stuff

The firmware is written in CircuitPython using the [KMK firmware framework](https://github.com/KMKfw/kmk_firmware). It handles all the key mappings and gets the macropad talking to Photoshop.

### Mapped Shortcuts

- `Ctrl + Z` → Undo
- `Ctrl + Shift + Z` → Redo
- The rest? Totally up to you.

📁 Firmware lives in: `/Firmware/main.py`

### Setup Instructions

1. Flash KMK to your XIAO RP2040
2. Drop `main.py` into the KMK folder on the device
3. Plug it in, fire up Photoshop, and go make cool stuff

---

## 📦 Bill of Materials (BOM)

| Item                        | Qty | Notes                       |
|----------------------------|-----|-----------------------------|
| Seeed Studio XIAO RP2040   | 1   | The microcontroller         |
| Mechanical Switches (MX)   | 4   | Go with your favorites      |
| Custom PCB                 | 1   | Designed in KiCad           |
| 3D Printed Case (Top + Bottom) | 1 set | Optional color flair 😉     |
| Keycaps                    | 4   | Any MX-compatible set       |
| Wires/Solder               | —   | Standard assembly stuff     |

---

## 🗂️ Repo Structure

