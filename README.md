# Anycubic i3 Prusa Clone - Marlin 1.1.x Configuration / Settings

This repository contains the Marlin firmware configuration for the Anycubic i3 Prusa clone with the following features:

- **Dual Z Motors:** Both Z motors are connected and configured to synchronize the movement of the Z-axis.
- **Limit Switches:** A single limit switch is used for each axis (X, Y, Z).
- **Cooling Fan:** Adjustments can be made for specific cooling needs.
- **Heatbed:** The heatbed is configured for printing with PLA. You may need to adjust the temperature settings based on your filament type and requirements.

### Motivation

I created this configuration because the Anycubic i3 Prusa clone is hard to find nowadays. However, I still use and repair mine, and I wanted to share this to help others who might be in a similar situation. By sharing this, I hope to help those that try desperately searching for configurations related to this printer.
  
### Firmware Configuration
The Marlin files for this setup can be downloaded from the official Marlin GitHub repository. 
The configuration files provided here have been optimized for the Anycubic i3 Prusa clone with dual Z motors and a single limit switch for each axis.

## Image

![Anycubic i3 Prusa Clone](https://testbericht.guru/wp-content/uploads/2016/09/Anycubic-Prusa-i3-3D-Drucker1.jpg)

*Source: [Testbericht Guru](https://testbericht.guru/)*

## Installation

To use this configuration:
1. Download the Marlin 1.1.x directory.
[Marlin 1.1.x on GitHub](https://github.com/MarlinFirmware/Marlin/tree/1.1.x)
2. Open the `Marlin.ino` file in the `Marlin-1.1.x/Marlin/` directory with the Arduino IDE.
3. Replace the `Configuration.h` and `Configuration_adv.h` files.
4. Customize the settings if needed.
(As Board you can Select Arduino Mega or Mega 2560 if you have the Trigorilla board)
5. Compile and upload the firmware to your Anycubic i3 Prusa clone using the Arduino IDE. 

## License

Feel free to use this configuration together with Marlin and adhere to the rules provided by them.

## Acknowledgments

- [Anycubic](https://www.anycubic.com) for producing the Anycubic i3 Prusa clone.
- The Marlin development team for their continuous work on the firmware.
