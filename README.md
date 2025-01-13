# Anycubic i3 Prusa Clone - Marlin 1.1.x Configuration

This repository contains the Marlin firmware configuration for the Anycubic i3 Prusa clone with the following features:

- **Marlin 1.1.x** firmware version
- **Dual motors** for height (Z-axis)
- **Single limit switch** for each axis (X, Y, Z)

### Motivation

I created this configuration because the Anycubic i3 Prusa clone is hard to find nowadays. However, I still use and repair mine, and I wanted to share this to help others who might be in a similar situation. By sharing this, I hope to contribute to the community and keep the printer running for as long as possible
  
## Configuration

### Hardware Setup
- **Dual Z Motors:** Both Z motors are connected and configured to synchronize the movement of the height axis. This helps maintain a level print bed and provides better Z-axis stability.
- **Limit Switches:** A single limit switch is used for each axis. This simplifies the setup and configuration while still ensuring precise endstop functionality.

### Firmware Configuration
The Marlin files for this setup can be downloaded from the official Marlin GitHub repository. 
The configuration files provided here have been optimized for the Anycubic i3 Prusa clone with dual Z motors and a single limit switch for each axis.

## Image

![Anycubic i3 Prusa Clone](https://testbericht.guru/wp-content/uploads/2016/09/Anycubic-Prusa-i3-3D-Drucker1.jpg)

*Source: [Testbericht Guru](https://testbericht.guru/)*

## Installation

To use this configuration:
1. Download the Marlin directory.
2. Open the `Marlin.ino` file in the `Marlin-1.1.x/Marlin/` directory.
3. Replace the `Configuration.h` and `Configuration_adv.h` files.
4. Customize the settings if needed.
5. Compile and upload the firmware to your Anycubic i3 Prusa clone using the Arduino IDE or PlatformIO.

## License

Feel free to use this configuration together with Marlin and adhere to the rules provided by them.

## Acknowledgments

- [Anycubic](https://www.anycubic.com) for producing the Anycubic i3 Prusa clone.
- The Marlin development team for their continuous work on the firmware.
