# 555 Timer Based Astable Multivibrator PCB Design

A manufacturing-ready, optimized 2-layer PCB layout for a 555 Timer Astable Multivibrator circuit, designed using **KiCad 8.0**. This project demonstrates industry-standard PCB design practices, including schematic capture, component placement optimization, ground plane design, and DRC compliance.

---

## 🚀 Key Technical Specifications & Features
* **Component Placement:** Optimized for minimal trace lengths and efficient routing paths.
* **Layer Count:** 2-Layer PCB (Top and Bottom Copper).
* **Power & Grounding:** Integrated a dedicated **Ground Plane (GND Pour)** on the copper layers to ensure signal integrity and minimize electromagnetic interference (EMI).
* **Design Rule Check (DRC):** 100% compliant with industry manufacturing constraints (**0 Errors / 0 Warnings**).
* **Fabrication Ready:** Standard **Gerber (X2)** and **Excellon Drill files** generated for seamless manufacturing.

---

## 🛠️ Visuals & Design Layout

### 1. 3D Render View
<img width="3450" height="1886" alt="led flasher 3D" src="https://github.com/user-attachments/assets/a14cd973-b6a2-4264-b440-6c5a44501012" />


### 2. PCB Layout
#### Top Layer Layout
<img width="1313" height="1716" alt="Screenshot (19)" src="https://github.com/user-attachments/assets/24c7ae24-a1f0-4285-91fc-3caea8d63c78" />

#### Bottom Layer Layout
<img width="1283" height="1713" alt="Screenshot (18)" src="https://github.com/user-attachments/assets/9e566e81-e54f-4e72-b053-0f4eb5e56556" />

---

## 💡 Engineering Challenges & Key Learnings
* **Ground Net Alignment:** Initially encountered DRC errors regarding unconnected ground pins. Solved by correctly binding the copper zone boundaries to the `GND` net, allowing automated copper flow across all ground pads.
* **Isolated Copper Islands:** Fixed potential manufacturing issues with isolated copper pours by tuning the zone properties and enabling automated island removal, maintaining a clean and effective ground return path.
* **Thermal Relief vs Solid Connections:** Analyzed pad connection types to balance between robust electrical connectivity and ease of manual soldering.

---

## 📂 File Structure
* `led flasher.kicad_sch` - Schematic capture file.
* `led flasher.kicad_pcb` - PCB Layout file.
* `Gerbers.zip` - Production-ready Gerber and Drill files for manufacturing (compatible with JLCPCB, PCBWay, etc.).

---
*Designed with 💻 using KiCad.*
