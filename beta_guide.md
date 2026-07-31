# Beta Guide

## OS
https://github.com/ros-realtime/ros-realtime-rpi4-image/releases/tag/24.04.2_v6.8.4-rt11-raspi_ros2_jazzy



## Beta RCB motherboard
**The mainboard have some modifications on them, cut traces or soldered wires. DO NOT remove or try to fix them this beta batch of pcbs had some mistakes that were fixed that way!**

## Setting up the motors with motorgui.com

* Go to [motorgui.com](motorgui.com)
* Go to the update firmware tab. Connect via USB to serial adapter to your driver
* Flash the latest firmware for stepfoc
* Exit firmware update, connect to gui via uart transport on the panel on the left side.
* Apply #default to your motor
* Go to preset tab and apply preset depending on what motor you are using. (preset for J1 is is Joint 1 (base) and so on...)
* #Save that
* In tune & calibrate press "Run #Cal" and calibrate your motor
* #Save 
* Do this for each of the PAR6 motors
 

## Beta RCB Mainboard — What to Expect
The PCBs ship flashed with RCB code (release v0, available on GitHub) and have been lightly tested. As an early v0 batch, the PCBs have some visible modifications — removed traces and jumper wires — that are required for proper operation. These do not affect the robot's performance.
Below is a summary of the known issues, all of which have been addressed on the boards before shipping:
K1 footprint / relay — Wrong footprint; relay is closed by default on power-on (should be open)
Q1 — Requires a jumper wire
D11 & D12 — Require jumper wires
E-stop connectors — Wiring is swapped; 2 E-stop pins need to be connected across the 2 connectors
R63 — Swapped to 1.47 kΩ
Trace cuts — Some traces need to be cut for proper operation (between the 2 green connectors and near J19)
