# About
This repo is for my own mod project aimed at updating an old kinesis contured model 100, using the Pillz Mod boards for both the thumb clusters and replacing the main PCB with the Pillz Mod.
My keyboard keywells do not match the wiring expected by Pillz Mod, so I will need my own firmware, documented here.

# Keywell wiring
I have traced out the keywells using a multimeter as follows:

## Right Keywell

|        | Pin 1 | Pin 2  | Pin 3 | Pin 4 | Pin 5 |
| ------ | ----- | ------ | ----- | ----- | ----- |
| Pin 6  | '     | RSHIFT | ]     | 6     |       |
| Pin 7  | \     | p      | /     | k     | i     |
| Pin 8  | -     | 0      | ;     | ,     | 8     |
| Pin 9  | 9     | .      | [     | DN    | UP    |
| Pin 10 | o     | l      |       | 7     | m     |
| Pin 11 |       |        |       | u     | j     |
| Pin 12 |       |        |       | n     | h     |
| Pin 13 |       |        |       |       | y     |

## Left Keywell

|       | Pin 9 | Pin 10 | Pin 11 | Pin 12 | Pin 13 |
| ----- | ----- | ------ | ------ | ------ | ------ |
| Pin 8 |       |        | `      | LSHIFT | CAPS   |
| Pin 7 | e     | d      | z      | q      | TAB    |
| Pin 6 | 3     | c      | a      | 1      | =      |
| Pin 5 | RIGHT | LEFT   | \      | x      | 2      |
| Pin 4 | v     | 4      |        | s      | w      |
| Pin 3 | f     | r      |        |        |        |
| Pin 2 | g     | b      |        |        |        |
| Pin 1 | t     | 5      |        |        |        |

# Additional jumper wires

The Pillz Mod does not have all of its input pins wired to the processor. I have added these wires:

- J3 pin 5 -- U2 pin 7
- J3 pin 11 -- nice!nano P1.01
- J4 pin 4 -- J9 pin 1
- J4 pin 9 -- J9 pin 2

# Open Questions

1. Do the jumper locations make sense? We will have to trace out the Pillz Mod board to figure out whether these jumpers make sense 
2. Can we change the config in this repo to drive the keyboard correctly?

