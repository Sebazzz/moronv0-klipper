# Voron V0.2r1 klipper config

My Voron V0.2r1 klipper configuration based on [the LDO motors Voron V0.2-S1 kit](https://docs.ldomotors.com/en/voron/voron02/BOM/RevA+). It assumes the presence of the LDO Picobilical board, and that the Raspberry PI itself [has also been set-up as a Klipper MCU](https://www.klipper3d.org/RPi_microcontroller.html).

Read more [on my Voron build on my website](https://damsteen.nl/blog/2023/12/29/ldo-voron-v02-build-notes).

## Features

- Split all the important configurations (like sensorless homing) to separate config files
- Use audio cues for important events like filament loading and print start
- Bed lightning represents the printer state
- Filament sensor auto-loads filament
- Support gcodes
   - M300 *beep*
   - M600 *filament change*

## Usage

Download all the files by going to the green "Code" button, and then selecting "Download ZIP".
Then upload all the configurations to your Klipper instance.

Then modify the MCU paths in [`configs/mcu.cfg`](./configs/mcu.cfg) to point to your MCUs.