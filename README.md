# A4 CNC Pen Plotter Machine

DIY A4 CNC Pen Plotter Machine using Arduino UNO, GRBL firmware, CNC Shield, NEMA17 stepper motors, and a servo-based pen lifting system for automated drawing and G-code plotting.

---

# Features

* A4 size plotting area
* X-Y axis movement system
* Servo based pen up/down mechanism
* GRBL 1.1 firmware support
* Inkscape compatible workflow
* G-code based drawing system
* Arduino UNO based control system
* CNC Shield support
* GT2 timing belt movement system

---

# Components Used

## Mechanical Components

1. Arduino Uno
2. CNC Shield
3. Stepper Motor Driver (A4988 / DRV8825)
4. Jumper Wires
5. DC Female Power Port
6. 2020 Aluminum Profile (X-axis)
7. 2040 Aluminum Profile (Y-axis)
8. M5, M4, M3 Nuts and Bolts
9. M5 Self-lock Screws
10. NEMA 17 Stepper Motor (48mm)
11. Servo Motor
12. Eccentric Spacer
13. 3D Printed Parts
14. Laser Cut Acrylic Parts
15. 12V 10A SMPS Power Supply
16. POM Wheels with Bearings
17. Timing Belt (GT2)
18. GT2 Pulley
19. Mounting Base Board (Wood/MDF)
20. Cable Management (Zip ties, Sleeves)

## Electrical Components

21. 5mm DC Connector Barrel Jack
22. 5mm DC Connector Socket
23. AC Wire
24. DC Wire
25. AC Plug
26. USB Cable
27. Power Switch

---

# Software Used

* Arduino IDE
* GRBL 1.1 Firmware
* Inkscape
* LaserGRBL
* Universal Gcode Sender (UGS)
* 4xiDraw Extension

---

# Wiring Overview

## X-Axis

* NEMA17 Motor -> X-axis port on CNC Shield

## Y-Axis

* NEMA17 Motor -> Y-axis port on CNC Shield

## Servo Motor

* Signal -> D11
* VCC -> 5V
* GND -> GND

## Power Supply

* 12V SMPS -> CNC Shield power input

## USB Connection

* PC -> Arduino UNO

---

# GRBL Installation

1. Install Arduino IDE
2. Download GRBL firmware
3. Add GRBL ZIP library
4. Open:
File -> Examples -> grbl -> grblUpload

5. Select:

Board -> Arduino UNO
Port -> Correct COM Port

6. Upload firmware

---

# Pen Servo Commands

## Pen UP

M3 S30

## Pen DOWN

M3 S90

# Creating G-code Using Inkscape

1. Create or import design in Inkscape
2. Select all objects
3. Convert objects to path:
Path -> Object to Path

4. Open:
Extensions -> 4xiDraw -> 4xiDraw Control

5. Configure:
* Pen Up Position
* Pen Down Position
* Servo Delay

6. Click Apply
7. Save generated G-code file

---

# Uploading G-code to Machine

1. Open LaserGRBL
2. Select COM port
3. Set baud rate to: 115200
4. Connect to Arduino UNO
5. Open G-code file
6. Preview drawing
7. Start plotting

---

# Testing

## Stepper Motor Test
G0 X10
G0 Y10

## Servo Test
M3 S30
M3 S90

---

# Future Improvements

* Wireless control system
* ESP32 upgrade
* Auto homing system
* Laser engraving support
* Higher plotting speed
* Better cable management

---

# Tags

Arduino
GRBL
CNC
Pen Plotter
A4 Plotter
Inkscape
G-code
NEMA17
DIY CNC
Servo Motor

---

# Author

Rashid Ahmmed
