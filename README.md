## Overview

 This repository contains custom firmware files for the [BT60](https://www.polarityworks.com/bt60) mechanical keyboard PCB. The key layout is inspired by the Happy Hacking Keyboard, with a few customizations to optimize [my workflow](https://github.com/akarez/macintosh) in the Binary Space Tiling Window Manager.

## Layers
  
### Base

 The base layer differs form the HHKB layout in having no FN key next to the right SHIFT. Instead, the space key acts as the FN key when held, and as SPACE when pressed once. Rightmost and leftmost of the bottom row are the ALT keys. This position allows for better ergonomics when pressing key chords in BSPWM. Lastly the size of the CMD keys is 1.5U since it is my most used key.

```
  -------------------------------------------------------------
 | esc | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 0 | - | = | \ | ` |
 | tab  | Q | W | E | R | T | Y | U | I | O | P | [ | ] | bspc |
 | ctrl  | A | S | D | F | G | H | J | K | L | ; | ' |   enter |
 | shift   | Z | X | C | V | B | N | M | , | . | / |     shift |
 | alt | fn1 | cmd |      space/fn1          | cmd | fn2 | alt |
  -------------------------------------------------------------
```

### Function

 The function layer has the usual media que function keys, and since the base layer does not have arrow keys, I find that pressing SPACE with the thumb and the vim keys HJKL is the best solution.

```
  -------------------------------------------------------------
 |     |f1 |f2 |F3 |f4 |f5 |f6 |f7 |f8 |f9 |f10|f11|f12|   |   |
 |      |   |   |   |   |   |   |   |   |   |prs|   |   |      |
 |       |vlm|vl-|vl+|   |   |lft|dwn|up |rgt|   |   | bootldr |
 | caps    |brm|br-|br+|   |   |   |   |   |   |   |           |
 |     |     |     |                         |     |     |     |
  -------------------------------------------------------------
```
 
 ### Bluetooth

 The bluetooth layer allows for switching between three devices, but the PCB currently supports up to five. The ESC key is mapped to Bluetooth Clear, which removes the device paired to the current profile. To switch between profiles use numbers 1, 2, and 3.
 
```
  -------------------------------------------------------------
 |btclr|bt1|bt2|bt3|   |   |   |   |   |   |   |   |   |   |   |
 |      |   |   |   |   |   |   |   |   |   |   |   |   |      |
 |       |   |   |   |   |   |   |   |   |   |   |   |         |
 |         |   |   |   |   |   |   |   |   |   |   |           |
 |     |     |     |                         |     |     |     |
  -------------------------------------------------------------
```

## Installation

 If you would like to replicate my configuration, set your PCB in bootloader mode and paste the bt60.uf2 file into the device. To make your own custom keymap follow the instructions in the Polarity Works [github repo](https://github.com/ReFil/zmk-config).
