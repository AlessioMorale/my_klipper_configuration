# Printer configuration for Klipper
This repository contains my current printer confiuguration for [Klipper](https://www.klipper3d.org/)

The printer has the following features:

- Cartesian kinematic, based on the PS3Steel frame
- 0.9° Steppers for X,Y and extruder, 1.8° for both Z
- physical endstop (switch on X, optical on Y)
- E3D V6 + Bondtech Extruder, Part Fan(FAN0 output)
- BLTouch (clone)
- TMC2130 on all axis, with one driver for each Z motor (dual Z)
- Thermistor+Fan for the enclosure (chamber, Heater1 and E3 pins)
- Hot end(FAN1 output) and controller(FAN2 Output) fan connected to a board fan output.
- Case light (Heater2 output)
- PSU control (J46, pin 4, PC9)
- Bigtreetech SKR pro 1.1
- Bigtreetech TFT24 display in 128x64 emulation (need to be updated to a recent version to work with klipper)

Firmware is split in several files for each logical section. Additionally the printer.cfg file is only used as a proxy for config.cfg.
This avoid risks to overwrite any calibration within printer.cfg
