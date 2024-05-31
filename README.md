# Dell charger emu ds2502
Dell charger emulator of DS2502. Based on OneWireHub project: [DS2502_DELLCHG](https://github.com/orgua/OneWireHub/tree/main/examples/DS2502_DELLCHG)

## Features

Now, you can select messages for different PSU wattages without reprogramming MCU. 

## HOWTO
1) To select wattage:
   - 45w -> short pin 4 to the ground
   - 65w -> short pin 6 to the ground
   - 90w -> short pin 9 to the ground
   - 130w -> no pins (4, 6, 9) are shorted to the ground
2) Powerup MCU

To change message:
- poweroff MCU
- make changes with pins
- powerup MCU

## Circuit recommendations
- connect to data-pin 10k pull-up to 3.3V

## Hardware
Sketch works on:
- Arduino UNO, Arduino Nano
- Arduino clones: LGT8F328P (library: https://raw.githubusercontent.com/dbuezas/lgt8fx/master/package_lgt8fx_index.json)

Laptops compatible:
- Dell 3567
- Dell 3576
- Dell 3585
