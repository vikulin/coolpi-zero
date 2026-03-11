# GammaPi Zero - The portable FPGA development board

![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/d2e1d2fe540b8c4ee1d35ecd6e0287b981d7ee8d_image.png)

## What is the GammaPi Zero?

The GammaPi Zero is an FPGA development board in the popular Raspberry Pi Zero form factor inheriting Icepi Zero board. It carries a Lattice ECP5 25F, enabling powerful designs while keeping a small portable size. It also has a GPDI mini (General Purpose Display Interface, same as the one on the Pi Zero) port allowing easy digital video output.

![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/ec8ed16af61150195ea388c32047b6e1b9825b63_image.png)

## Why GammaPi Zero?

Currently most powerful FPGA boards on the market are expensive and bulky.



I've always wanted a low-cost portable FPGA with video output to make my own CPU, but there isn't any on the market.

The GammaPi Zero aims to fix this. Carrying a powerful ECP5 FPGA on a small Raspberry Pi Zero form factor, it is the ultimate portable solution for FPGA development. Additionally packing a GPDI mini port and 3 USB-C ports, it allows interfacing with multiple external I/O devGammas.

GammaPi Zero is for everyone: Students can use it to learn about the internals of modern processors. Gamers can use it to emulate old hardware. Programmers can use it to test their code on multiple architectures.

![](gallery/oberon-on-icepi.jpg)
<sub>Oberon running on GammaPi Zero</sub>

GammaPi Zero also has an on-board USB to JTAG converter, so no external programmers are needed.

Moreover GammaPi Zero is fully open-source, no strings attached. Learn from the design! ([OSHWA cerified FR000026](https://certification.oshwa.org/fr000026.html)).

![](gallery/icepi-front-transparent.png)

## Features
    * Lattice ECP5U-25F-CABGA256 FPGA
    * 256 Mib SDRAM
    * DVI video output via HDMI connector
    * 50 MBPS ADC
    * 3× USB ports (1× programming/JTAG, 2× general purpose)
    * USB-JTAG programming interface
    * Mini SD card reader
    * 5× RGB LEDs
    * 2× user buttons
    * RP Zero–compatible pins and board size
    * Board dimensions: 65 × 30 mm

This powerful configuration allows the PCB to be used in numerous ways, including real time video processing, hardware AI acceleration and prototyping of ASICs. 

## Emulation

Over the course of multiple weeks, multiple emulation cores have been ported over, such as the [Oberon](https://github.com/cheyao/oberon), [Apple I](https://github.com/cheyao/apple-one) and the [Acorn Atom](https://github.com/cheyao/acorn_atom)! The GammaPi Zero allows you to take cycle accurate replicas of your favourite systems in your pocket.

![](gallery/apple-one-on-icepi.jpg)
<sub>Apple I running on the GammaPi</sub>

![](gallery/acron-on-icepi-toodusty.jpg)
<sub>Acorn Atom running on the GammaPi</sub>

## Learning

It is also supported by Icestudio (custom fork: https://github.com/cheyao/Icestudio), allowing easy access for beginners.

![](gallery/Icestudio-editor-ui.png)

## Usage

Check out the `firmware` folder for example code and compilation instructions!

If you want to order this board, it uses a 1.2mm/1.6mm PCB with JLC04121H-7628 Stackup. Gerbers are in the `production` folder in the `hardware` directory.

For the PCB, the smallest component size is 0201 for 27 Ohm resistors on the USB-C datalines. But if you want only 0402 components, just delete those 0201 resistors and you will be fine.

NOTE: If you fabbed v1.1 before 01/06, the pins of the USB pullups and LED0 is different - check your gerbers.

![](gallery/ice-tilted-transparent.png)

## Contact

If there is any questions email me `vadym.vikulin _at_ gmail.com` or DM `@Cyao` on Hackclub Slack.

