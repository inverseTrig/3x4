# 3x4

A small macropad in a 3x4 layout powered by [KMK](http://kmkfw.io/). If you are new to handwiring, [worry not](https://geekhack.org/index.php?topic=87689.0).

![Diagonal view](/images/diagonal.jpg)
![USB port view](/images/usb_port.jpg)

## Required Parts

| Part                                                                                       | Qty | Description                                                      |
| ------------------------------------------------------------------------------------------ | --- | ---------------------------------------------------------------- |
| [RP2040 Zero](https://a.aliexpress.com/_mP1tyzy)                                           | 1   | Micro controller board                                           |
| MX-style switches of your choosing                                                         | 12  | I used Outemu Lemon/Limes.                                       |
| [1N4148 Diodes](https://a.aliexpress.com/_msALIYo)                                         | 12  | You need these for handwiring                                    |
| [M2 x 6mm hex female-to-female brass standoff (spacer)](https://a.aliexpress.com/_mO2uQEM) | 2   | This is what supports/holds down the plate and the case together |
| M2 x 6mm [flat top screws](https://a.aliexpress.com/_mqwmkN6)                              | 2   | Plate-side that goes with the brass standoff                     |
| M2 x 6mm [countersunk screws](https://a.aliexpress.com/_msph8rW)                           | 3   | Holdes the case and plate together. Also holds the MCU down.     |
| M2 hex [nut](https://a.aliexpress.com/_m0uPPtO)                                            | 1   | Holds the MCU down                                               |

## Firmware

I used [KMK](http://kmkfw.io/) which runs on [CircuitPython](https://circuitpython.org/). If you are new here, you should take a look at the [Getting Started](http://kmkfw.io/docs/Getting_Started) section of KMK.

## Changing the keymap

To change the keymap of the keyboard, press the most top-left key (default mapped to `Q`), and then connect it to the computer. There will be a USB shown in your Finder/File Explorer. Inside the USB, there's a `code.py` that can be modified. Here's all the [keycodes](http://kmkfw.io/docs/keycodes/) supported by KMK. If you're looking for a more complex behavior (ie. combos, layers, hold-tap, mouse keys, etc), check out the [modules](http://kmkfw.io/docs/modules/) section.

Note: Do not modify the `boot.py` as it would change the key required to have the USB show up in Finder/File Explorer.
