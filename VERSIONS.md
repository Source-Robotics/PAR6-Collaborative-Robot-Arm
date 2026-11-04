# PAR6 versions

Which PAR6 you have, and which files, software and manual go with it.

## Releases

There is no release yet. PAR6 is in beta: the files on the main branch of this repository (the print files, the BOM,
the assembly manual) are the latest, and the instructions, the code and the 3D print files may still change.

## The beta

| Part | In the beta | More |
|---|---|---|
| The arm | the files on the main branch; no hardware revision released yet | [Hardware revisions](https://docs.source-robotics.com/par6/latest/par6/appendices/hardware-revisions/) in the manual |
| Control box mainboard | the beta batch, shipped flashed with the RCB code release v0; it has cut traces and jumper wires that fix known mistakes of the batch: do not remove them | [beta guide](beta_guide.md) |
| Joint drives | STEPFOC, flashed with the latest STEPFOC firmware and calibrated with [motorgui.com](https://motorgui.com) | [beta guide](beta_guide.md) |
| Operating system | [ros-realtime-rpi4-image 24.04.2_v6.8.4-rt11-raspi_ros2_jazzy](https://github.com/ros-realtime/ros-realtime-rpi4-image/releases/tag/24.04.2_v6.8.4-rt11-raspi_ros2_jazzy), on the control box's Raspberry Pi 5 | [beta guide](beta_guide.md) |
| Runtime | the manual describes [RCB-Runtime v1.1.1](https://github.com/Source-Robotics/RCB-Runtime/releases/tag/v1.1.1) | [Downloads and files](https://docs.source-robotics.com/par6/latest/par6/cad-files/) |
| Manual | PAR6 Hardware Manual SR-1001, revision 2026.A, a draft; for the PAR6 arm, revision v1.x | [the manual](https://docs.source-robotics.com/par6/) |

## Which version do I have?

| | Where to see it |
|---|---|
| Control box mainboard | the beta batch carries the fixes the [beta guide](beta_guide.md) lists (K1, Q1, D11 and D12, the E-stop connectors, R63, the trace cuts) |
| Runtime | Dashboard → System Info → Versions |
| Drive firmware | Dashboard → Motor tab, or `get_hardware`; runtime 1.1.1 supports 103 or newer |

## What works together

The runtime, the Python client, the drive firmware, the control box PCB, the arm and grippers, the models and the
operating system image of each runtime release:
[Versions and compatibility](https://docs.source-robotics.com/par6/latest/support/versions/) in the manual.
