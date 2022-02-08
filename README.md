# Marlin-2.0.x_config

Marlin 2.0.x custom configuration files for my upgraded Ender 3 Pro.
These files are specific to my setup and are provided for educational purposes only.
Use at you own risk!

## Configuration
* Ender 3 Pro or Ender 3 V2
* Creality V4.2.2 or V4.2.7 mainboards
* Marlin 2.0.9.3 firmware
* E3D V6 hotend
* BondTech BMG extruder
* BLTouch Auto Bed Leveling sensor (Connected to the dedicated 5 pins connector of the Creality V4.2.7 board, not to the Z min stop pins)

## How to compile & build?
* Download the Marlin source code (https://marlinfw.org/meta/download/ or https://github.com/MarlinFirmware/Marlin)
* Overwrite the default configuration files in the Marlin directory (Configuration.h, Configuration_adv.h etc.) with the files provided
* Install Microsoft Visual Studio Code + PlatFormIO IDE (see https://marlinfw.org/docs/basics/install_platformio_vscode.html)
* Install the "Auto Build Marlin" extension (see https://marlinfw.org/docs/basics/auto_build_marlin.html)
* Compile & Build Marlin with a single click using the Auto Build Marlin extension (see see https://marlinfw.org/docs/basics/auto_build_marlin.html)

## How to install?
* Copy the firmware binary (e.g. .pio/build/STM32F103RET6_creality/firmware-20210906-101846.bin) to the root directory of an SD card. Make sure you use always a new filename!
* Insert the SD card into your printer and power it on. This should update the firmware with the binary provided

## How to check the firmware version?
On the printer, click on About Printer > Printer Info

## What to do next?
* Initialize EEPROM (Configuration > Advanced Settings > Initialize EEPROM)
* Restore all settings to their default values (Configuration > Restore Defaults)
* Update the Z offset (Configuration > Probe Z Offset). This is the distance between nozzle and the probe tripping point. The expected value should be between -2.0 mm and -4.0 mm.
* [Optional] Enable firmware retractions (Configuration > Retract > Auto-Retract) and adjust retraction settings as needed
* Save the current configuration in EEPROM (Configuration > Store Settings)
* Enjoy some good old retro games! (About Printer > Games)



 





