# Slim Hitbox Enclosure

This repository contains 3D models, assembly instructions, and detailed documentation for building a compact, 3D-printed hitbox-style arcade controller.

## Project Overview

This Slim Hitbox Enclosure provides a slim, portable alternative to traditional arcade controllers, making it ideal for travel and easy setup. It supports 3D printing, simple assembly, and an ergonomic design. 

> **Note**: Version 1 is exclusively in the southpaw (left-handed) layout. Currently, there is no orthodox (right-handed) version.

## Features

- **Compact and Slim Design**: A low-profile layout optimized for easy handling and storage.
- **3D Printable Components**: Fully printable in standard PLA/ABS materials.
- **Ergonomic Design**: Includes a wrist rest for comfort.
- **Comfortable Assembly**: Chamfered screw holes provide a smoother finish.

## Attributions

This project uses GP2040 to enable the microcontroller to function as a game controller. Special thanks to the knowledgeable members of the GP2040 Discord community for their assistance and expertise, and to the helpful contributors on the r/pcb subreddit for reviewing the board's usability before it was sent for production.

## Prerequisites

- Access to a 3D printer and filament (PLA, ABS, or similar recommended)
- Personal Computer with USB port
- Soldering equipment and basic assembly tools

## Instructions

1. **PCB Manufacturing**: Have the PCB manufactured using the Gerber files in the `fab` folder.
2. **Download STL Files**: Access the STL files from the `models` directory.
3. **Slice and Print**: Use slicing software like Cura or PrusaSlicer to prepare and print the models. Adjust settings as needed based on your specific printer and filament.
4. **Assemble**: Follow the assembly instructions below.

## Parts List

- **Buttons**: 9x 30mm buttons, 3x 24mm buttons
- **Keycaps**: 5x keycaps
- **Panels**: 1x top panel, 1x bottom panel
- **Cables**: 1x Micro USB male to USB male cable ([link](https://www.amazon.com/gp/product/B08BZD66H4/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1)) 1x, 1x USB female to USB male cable
  1. (length should match your preferred distance to console or PC)
- **Hardware**: 6x M3 x 20mm screws, 6x M3 bolts
- **Feet**: 6x printed feet
  1. (ensure bolts fit snugly)
- **Electrical Components**:
  - 1x Raspberry Pi Pico
  - 17x MX Cherry or MX Cherry-compatible keyswitches
  - 2 rows of 100-pin male header pins ([link](https://www.amazon.com/dp/B06ZZN8L9S?ref=ppx_yo2ov_dt_b_fed_asin_title))
  - 1x PCB

## Assembly Instructions

1. **Prepare Feet**: Apply a strong bonding agent to the inner walls of each foot, then insert bolts into all six printed feet.
2. **Microcontroller Setup**: Solder male header pins to the Pico microcontroller.
3. **PCB Assembly**: Solder the microcontroller to the PCB using the header pins.
4. **Keyswitch Installation**: Solder all 17 keyswitches onto the PCB.
5. **Cable Guide**: Attach the Micro USB to USB cable to the Pico and guide it through the channels in the top panel.
6. **Enclosure Assembly**: Place the PCB between the top and bottom panels.
7. **Secure Panels**: Screw the panels together and attach them with the feet.
8. **Install Buttons**: Attach all printed buttons, following the image shown below.

   ![Slim Hitbox Assembled](https://github.com/user-attachments/assets/6dd37290-5967-4847-8024-a1dc7b940e5e)

9. **Attach USB Cable**: Connect the USB female-to-male cable to the exposed USB head.

## Configuration

1. **Download Firmware**: Get the appropriate microcontroller `.uf2` file from the [GP2040 website](https://gp2040-ce.info/downloads/).
2. **Connect and Install Firmware**: Plug the USB cable into a PC, then drag the `.uf2` file into the storage device that appears in the file explorer when the hitbox is connected.
3. **Configuration Setup**: If the default layout is unsatisfactory, use the [web configurator](https://gp2040-ce.info/web-configurator/) to customize the button layout.
4. **Ready to Play**: Boot up your favorite fighting game and enjoy!


