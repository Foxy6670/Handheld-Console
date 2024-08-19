# Handheld Console (please suggest a better name)
## What is this?

This is a console designed with the people and nostalgia in mind - a console that anyone can tamper or screw around with, without worry of bricking it.

Users are encouraged to do whatever they want with it. You can design peripherals thanks to the expansion ports. You can build your own games and run them on real hardware. With enough luck and skill, you could probably even get online multiplayer working for some games. Who knows, you could probably get an OS up and running on this thing.

## What does it do?

It's a game console. It runs games and displays them on a 4" vertical Watchman-like CRT via composite video. You can likely get it to do much more than just that, though.

## Can I buy one?

No. At least, not yet. I'm not sure. However, planning files and spreadsheets will be available soon so you can build one for yourself.

## What are the specs?

It's using the RP2350 chip, which boasts a dual-core, dual-architecture processor (ARM and RISC-V), 520KB of RAM, 2MB of onboard BIOS storage, and has an external SD card slot that can utilize up to 4GB of storage, read and write. The CRT used (4" vertical CRT, Watchman-like) is the base of the console and what it's built around, and supports 128x96, 160x120, 256x192, 320x240, 400x300, 640x480, and 800x600. It has 2 expansion ports, one for SPI and another for i2c, both for custom peripherals not normally included with the system.
(The supported resolutions need a little more in-depth research, but these are resolutions normally supported by Composite.)

## What games will be included?

I'm not entirely sure yet. I'm thinking about making a Sonic the Hedgehog demo for this console, but this isn't confirmed.

## What is all the hardware this thing has?

- Heart of the console, Unknown Vertical CRT (Watchman-like)
- RP2350 Microcontroller
- Custom PCB (in the works)
- YMF825 (SPI bus 0; shared)
- Generic Latching Female SD Card Port (SPI bus 0; shared)
- Generic Headphone Jack
- Generic Potentiometer (x3) (Volume, Brightness, Contrast)* (I might have brightness and contrast be digitally controlled in the final version)
- Generic Speaker (2x)
- Generic Switch (3x) (Output (Internal/Composite out), Sound (headphone jack/speakers), Power (on/off))
- Generic Red LED
- Generic Green LED
- Generic Composite OUT
- Generic Button (x10) (U, D, L, R, 1, 2, 3, 4, Start, Select)
- Generic Female RCA Adapter
- "EVE 26V 18650 2550mAh 7.5A Battery" (x4, for estimated 36.72Wh (CRT uses 6W nominal, 7W peak, should give a few hours of runtime)
- Generic 4-pin adapter (for i2c 1, pin 0: +5V; pin 1: GND; pin 2: SDA; pin 3: SCL)
- Generic 6-pin adapter (for SPI 1, pin 0: +5V; pin 1: GND; pin 2: /CS; pin 3: SCLK; pin 4: MOSI; pin 5: MISO)
- Generic Lithium BMS with Type C Connector
- 3.3v to 12v boost converter/regulator
- 12v to 5v step-down converter
- 3.3v voltage regulator

## What's the estimated battery life?

Under full load with a full charge, I'd guess around 4 to 5 hours, but I haven't been able to test this yet.

### Feel free to ask any questions in the Issues tab!
