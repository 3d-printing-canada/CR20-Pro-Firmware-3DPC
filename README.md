# CR20-Pro-Firmware-3DPC
Updated Marlin firmware for the CR-20 Pro

## Overview

This update brings a few changes to the CR-20 Pro:

1) Updated and improved Z-offset consistency between prints
2) Live-Z adjust the Z offset during prints by clicking the select button 4 times on the printer. 
3) Overal reliability improvements (Marlin 2.0)

## Installation Procedure: 

XLoader is a program designed to upload firmwares to your 3d printer. Download XLoader from this source: http://www.hobbytronics.co.uk/arduino-xloader

1) Plug your printer into your computer
2) Open XLoader. Configure it with the following values: 
      - Hex File: Please download the "Cr20 Pro 3DPC Update.hex" from this repository
      - Device: MEGA(ATMEGA2560)
      - COM Port: The com port for your printer (should only be 1-2 there - try both if you don't have success at first)
      - Baud Rate: 115200
3) Press Upload.
