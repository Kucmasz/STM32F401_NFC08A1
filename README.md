# STM32 NFC Reader Project

## Project Description
This project utilizes the STM32 NUCLEO-F401RE board in conjunction with the NUCLEO-NFC08A1 NFC module to read NFC tags. The data retrieved from the tags are then transmitted over UART.

## Hardware
- **Boards:**
  - STM32 NUCLEO-F401RE
  - STM X-NUCLEO-NFC08A1

## Software
The project was initially migrated manually from the NUCLEO-L476RG based example to NUCLEO-F401RE board, using STM32CubeMX with X-CUBE-NFC6 SW Package.

Tested on STM32CubeMX version 6.11.1 and STM32CubeIDE version 1.15.1.

## Setup
1. Clone the repository to your local development environment.
2. Open the project in STM32CubeIDE.
3. Build the project and program the board using the build and run feature.

## Features
- Reading data from NFC tags.
- Transmitting read data through UART.

## How to Use
To begin, bring an NFC tag close to the NUCLEO-NFC08A1 reader. The tag's data will be read and sent via UART, which can be read using any UART terminal.

Example output in Minicom:
```
Welcome to X-NUCLEO-NFC08A1
Initialization succeeded..
NFCA Passive ISO-DEP device found. UID: 0423431AE87180
 Select NDEF Application: OK Data: 6F228520163AAEF998
```
