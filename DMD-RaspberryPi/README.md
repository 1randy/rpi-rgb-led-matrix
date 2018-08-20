Adapter PCB to support up to 3 panel chains
===========================================

   * Supports up to three panel chains for newer plus models and
     Raspberry Pi 2 that have 40 GPIO pins.
   * Uses HCT245 to level shift signals from 3.3V to 5V and shield
     the Raspberry Pi GPIOs from overloading.
   * Optional: Pads to power the Pi with 5V, including optional capacitor footprints.
   * Provides a way to choose the pinout for different kinds of 64x64 matrixes.
   * BOM:
     - 4x 74HCT245 or 74AHCT245 in 20-SOIC, 7.5mm package which should make
     it easy to hand-solder. Make sure to get the variant with the **T**: HC**T** or AHC**T**
     (there are also HC or AHC, don't use these).
     - 4x 100nF ceramic capacitor (0805 package)
     - 1x 10kOhm resistor (0805 package). Not critcial, just a pullup (2.2k .. 15k probably ok).
     - 3x 16pin IDC (=2x8) male receptible to connect the panels.
     - 1x 40pin female connector to connect to the RPi.
     - 1x (optional) 22μF .. 100μF capacitor for 5V rail.
     - 1x (optional) WAGO 2060 Cable Clamp

## Layout
![pcb-top][pcb-top]
![pcb-bot][pcb-bot]


## Schematic

![Schematic][schematic]

[pcb-top]: ./DMD-RaspberryPi_pcb_top.jpg
[pcb-bot]: ./DMD-RaspberryPi_pcb_bot.jpg
[schematic]: ./DMD-RaspberryPi.sch.png

