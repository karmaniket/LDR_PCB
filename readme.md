<h1 align="center">LDR Sensor PCB</h1>

This repository contains the KiCad design files, Gerber outputs, and documentation for a Light Dependent Resistor (LDR) sensor PCB. The project is intended for use in light-sensing applications and is suitable for both prototyping and production.

## Demo

***Click below for full KiCad tutorial***

[![Demo](https://img.youtube.com/vi/dt0KDcHqgbA/maxresdefault.jpg)](https://youtu.be/dt0KDcHqgbA)

## Applications

- Automatic window blinds
- Laser light security system
- Light-activated fans or doors
- Automatic street lights
- Smart lighting system
- Solar garden lights
- Energy saving system
- Smart curtains

> [!NOTE]  
> This PCB is suitable for personal projects. Significant modifications are needed for real-world or industrial applications.

## Project Structure

```bash
. 
├── ldr sensor.kicad_pcb                # KiCad PCB layout file
├── ldr sensor.kicad_sch                # KiCad schematic file
├── ldr sensor.kicad_pro                # KiCad project file
├── gerber/                             # Gerber fabrication outputs
```

## Fabrication Outputs

All Gerber files required for PCB fabrication are located in the [gerber/](gerber/) directory:

```bash

**Copper Layers:**
- `ldr sensor.kicad_pc_boards-F_Cu.gbr`          # Top copper layer
- `ldr sensor.kicad_pc_boards-B_Cu.gbr`          # Bottom copper layer
**Solder Mask:**  
- `ldr sensor.kicad_pc_boards-F_Mask.gbr`        # Top solder mask, Negative polarity
- `ldr sensor.kicad_pc_boards-B_Mask.gbr`        # Bottom solder mask, Negative polarity
**Silkscreen:**  
- `ldr sensor.kicad_pc_boards-F_Silkscreen.gbr`  # Top silkscreen
- `ldr sensor.kicad_pc_boards-B_Silkscreen.gbr`  # Bottom silkscreen
**Paste Layers:**  
- `ldr sensor.kicad_pc_boards-F_Paste.gbr`       # Top paste
- `ldr sensor.kicad_pc_boards-B_Paste.gbr`       # Bottom paste
**Board Outline:**  
- `ldr sensor.kicad_pc_boards-Edge_Cuts.gbr`     # Board outline
**Job File:**  
- `ldr sensor.kicad_pc_boards-job.gbrjob`        # job file for CAM automation
```

## Setup

### 1. Clone the repository

```bash
    git clone https://github.com/karmaniket/LDR_PCB.git
    cd LDR_PCB
```

### 2. Open in KiCad

- Make desired customizations
- In some cases, you may need to define custom footprints to match non-standard components
- THT (Through-Hole Technology) components were intentionally chosen for ease of prototyping and assembly, but you can substitute SMD (Surface-Mount Device) components if preferred

### 3. Requirements

```bash
    BC547 Transistor, 200 Ohm Resistor, LDR, Buzzer, LED, 9V Battery
```

### 4. Order the PCB

- Zip all files in the [gerber/](gerber/) directory except `.gbrjob`
- Upload the ZIP to your preferred PCB manufacturer (e.g., JLCPCB, PCBWay)

Use the following specifications:

- **Layers:** 2
- **Material:** FR4
- **Thickness:** 1.6mm
- **Copper Weight:** 1oz
- **Solder Mask:** Both sides
- **Silkscreen:** Both sides
- **Surface Finish:** As required

## License

This project is licensed under the MIT License. Feel free to use, modify and distribute with attribution.
