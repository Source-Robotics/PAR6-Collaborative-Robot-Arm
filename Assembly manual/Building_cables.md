# PAR6 cables

PAR6 robotic arm uses 2 types of cables:
* JST XH series for power delivery to motor drivers - 24 AWG or 22 AWG
* JST ZH series for CAN comms between motor drivers - 28 AWG


> [!NOTE]
>     **It is recommended to twist all CAN bus cables**

> [!WARRNING]
>     **If you are unsure if cables you bought from 3rd party stores are good orientation, lenght or type we recommended buying them from our store. Using wrong cables will damage and destroy your robot.**



If you want to build your own cables this document will provide you with a quick guide on how to build them.

Watch this video on cable assembly

## XH & ZH dual female head cables
These cables need to follow the **wiring diagram** (How wires are connected to the head) shown below! 

<img src="../BOM/BOM%20reference%20images/ZH_XH_cable_direction.png" alt="drawing" width="500">


These cables can be bought from multiple stores in different sizes.
Sizes we need for PAR6 are:
* 2 x 10cm XH dual female head/plug connector
* 2 x 10cm ZH dual female head/plug connector

* x x 23cm (difficult size to find use 25 or 30)


## XH series extension cables

[Video reference](https://youtu.be/GOb1vQsjfOs)

Parts needed:
* XH male connector
* XH female - female wire (or female - bare wire)
* Heat shrink tube

Cut one end of the XH female-female wire and keep the wire length at around 23cm.
Place heat shrink on the wires. Solder male XH connector to the wires. Follow the orientations on the image below. Heat the heat shrink tubes.

<img src="../BOM/BOM%20reference%20images/XH_series_extension_cable.png" alt="drawing" width="500">

## ZH series extension cables

[Video reference](https://youtu.be/GOb1vQsjfOs)

Parts needed:
* ZH male connector
* ZH female - female wire (or female - bare wire)
* Heat shrink tube

Cut one end of the ZH female-female wire and keep the wire length at around 23cm.
Place heat shrink on the wires. Solder male ZH connector to the wires. Follow the orientations on the image below. Heat the heat shrink tubes.

<img src="../BOM/BOM%20reference%20images/ZH_series_extension_cable.png" alt="drawing" width="500"/>

## Motor to Base Distribution PCB wire

These wires have a female head on one side and bare wires on the another. They connect directly to the Base Distribution PCB.

Parts needed:
* ZH female-female wire or female - bare wire 

Cut one end of the wire and keep the length of the wire at around **50cm**.


## Extension wire base -  Base Distribution PCB

These wires have a male head connector on one side and bare wires on the another. They connect directly to the Base Distribution PCB.

Parts needed:
* XH male connector
* ZH male connector
* Bare wires (2 colors black and white 24 AWG)

Solder male connectors the same way as when building ZH or XH extenstion cables. 

## PAR6 Robot cable (Robot base to RCB (Robot Control Box) cable)

[Video reference](https://youtu.be/QlNfWAga1l0)

Parts needed:
* [2 x GX16 4PIN connector female](https://s.click.aliexpress.com/e/_c3o4afqR)
* [Twisted Pair Shielded Cable 4 cores - 24AWG or 22AWG](https://s.click.aliexpress.com/e/_c34NcZIT)


Check the video tutorial [here](TODO)

<img src="../BOM/BOM%20reference%20images/GX16_disassembled.jpg" alt="drawing" width="500"/>

**Dissasemble the connector.**

<img src="../BOM/BOM%20reference%20images/GX16_numbering.jpg" alt="drawing" width="500"/>

**Connector has numbering on both sides.** 

<img src="../BOM/BOM%20reference%20images/GX16_numbering2.jpg" alt="drawing" width="500"/>

**When assembling the cable you solder pins 1-1, 2-2, 3-3, 4-4. Do that for the both sides of the cable!** 



> [!NOTE]
>     **Pins 1-4 need to be one wisted wire pair and pins 2-3 need to be another pair!**

## Robot base connector

<img src="../BOM/BOM%20reference%20images/GX16_POWER_CONNECTOR_RCB.png" alt="drawing" width="500"/>

On the robot arm side and Robot Control Box side the we use this pinout for X16 male connector!

Solder XH wire to the pins 1 and 4. Solder ZH CAN wires to pints 3 and 2. Keep wire length at around 10cm


## MSG & SSG48 gripper cable

Buy Official cables from Source Robotics: [Link](TODO)

Parts needed if DIY your own cable:

| Type | Length / Spec | Quantity | Description | Link |
|------|---------------|----------|-------------|------|
| 26 AWG cable | 0.15 mm², 4-wire twisted pair | 0.4 m | ~40 cm usually sufficient | [Link](https://s.click.aliexpress.com/e/_c4m3ggwn) |
| M8 4-pin male wire connector | — | 1 | [See reference image](../BOM/BOM%20reference%20images/M8%20male.png) |[Link](https://s.click.aliexpress.com/e/_c4OWHPKF) |
| M8 4-pin female wire connector | — | 1 | [See reference image](../BOM/BOM%20reference%20images/M8_female.png) | [Link](https://s.click.aliexpress.com/e/_c4OWHPKF) |


> [!NOTE]
>     **PAROL6 and PAR6 use different cables for SSG48 and MSG grippers. Using incorrect one can damage your robot**



<img src="../BOM/BOM%20reference%20images/Gripper_cable_contact layout.png" alt="drawing" width="500"/>


End result of this cable assembly needs to look like this:

<img src="../BOM/BOM%20reference%20images/cable_assembly.png" alt="drawing" width="500"/>


