# PiCade

PiCade is an open-source mini arcade machine built around a Raspberry Pi 4B. It includes two custom multiplayer games and can also be used with RetroPie (controller compatibility may vary). PiCade is designed as a compact, party-friendly console for up to 4 players.

## Status

Development in progress — hardware prototypes and software are actively being developed. Progress updates and hour logs are tracked in /docs/devlog.md.

## Key Features

- 7" touchscreen display (with optional HDMI output to a TV or external monitor)
- Up to 4 USB-C powered controllers
- Games written in Python using Pygame
- Controller firmware using Arduino or CircuitPython
- Auto-launches into a game menu on boot

## Hardware

- SBC: Raspberry Pi 4B
- Display: 7" touchscreen (connects directly to the Pi or use micro-HDMI to output to an external display)
- Controllers: 4 custom controllers powered over USB-C
- Case: Mini arcade-style cabinet

Notes:
- When using RetroPie, controller compatibility may differ depending on firmware and mapping.

## Software

- OS: Raspberry Pi OS (Lite) or a custom minimal OS image
- Game engine: Python + Pygame
- Controller firmware: Arduino or CircuitPython (depending on controller hardware)
- Boot behavior: System boots and auto-launches the PiCade game menu

## Getting Started (Development)

1. Prepare an SD card with Raspberry Pi OS (Lite) or your preferred image.
2. Install Python 3 and pip if not included.
3. Clone this repository:

   git clone https://github.com/AHuman328/PiCade.git

4. Install Python dependencies (example):

   pip install pygame

5. Run the game launcher or individual games from the project directory:

   python menu.py

(Adjust filenames and commands to match the repository layout.)

## Using with RetroPie

PiCade games may run on RetroPie, but custom controller firmware and mappings may be required. If controllers are not detected, check:

- Controller firmware is up to date
- USB mappings in RetroPie configuration
- That controllers are powered and enumerated by the Pi

## Development Notes

- Game code is implemented in Python and uses Pygame for rendering and input handling.
- Controller firmware prototypes use Arduino or CircuitPython. See controller folders (if present) for source and wiring details.

## Devlog

Progress updates and hour logs are tracked in `docs/devlog.md` for the Macondo hardware grant.

## Contributing

Contributions are welcome. Please open issues for bugs or feature requests. If you plan to submit code, open a pull request and include a description of your changes and testing steps.

## License

This project is licensed under the MIT License — feel free to remix and adapt it for your own projects.

## Credits

- Project: AHuman328
- AI assistance was used for code understanding, measurements, and review of technical details.

If you'd like, I can also:
- Add an example folder structure or TODO list in the README
- Create a CONTRIBUTING.md or CODE_OF_CONDUCT
- Add setup scripts to streamline dependency installation
