# Beta Guide

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
 