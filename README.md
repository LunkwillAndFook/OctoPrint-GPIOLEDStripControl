# OctoPrint-GPIOLEDStripControl

OctoPrint plugin that intercepts M150 GCode commands and controls LEDs connected to a custom driver board.

Implements the M150 command syntax from the latest Marlin.

        M150: Set Status LED Color - Use R-U-B for R-G-B Optional (W)
        M150 R255       ; Turn LED red
        M150 R255 U127  ; Turn LED orange (PWM only)
        M150            ; Turn LED off
        M150 R U B      ; Turn LED white
        M150 W          ; Turn LED white if using RGBW strips (optional)

## Setup

1. Connect driver board

2. Install via the bundled [Plugin Manager](https://github.com/foosel/OctoPrint/wiki/Plugin:-Plugin-Manager)
or manually using this URL:

    	https://github.com/LunkwillAndFook/OctoPrint-GPIOLEDStripControl/archive/master.zip

3. Restart OctoPrint

## Configuration

Configure the GPIO pins via the OctoPrint settings UI.

## Credit

Much of the code I have modified to make this work was shamelessly lifted from https://github.com/ozgunawesome/OctoPrint-PCA9685LEDStripControl.

## Disclaimer

This is **not** an official Google product.
