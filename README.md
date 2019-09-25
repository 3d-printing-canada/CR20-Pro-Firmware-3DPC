# CR20-Pro-Firmware-3DPC
Updated Marlin firmware for the CR-20 Pro

## Overview

This update brings a few changes to the CR-20 Pro:

1) Updated and improved Z-offset consistency between prints
2) Live-Z adjust the Z offset during prints by clicking the select button 4 times on the printer. 
3) Overal reliability improvements (Marlin 2.0)

## Operation Changes 

The procedure for setting up the Z offset is now different than the traditional CR-20 pro with these new firmware changes. Please follow the following procedure: 

### Setting the Probe Z Offset

1) Heat the printer up to 200 celcius on the nozzle, 60 on the bed
2) Auto home the printer
3) Move the printer's Z axis to zero. Make sure you have your paper underneath the nozzle before doing this
4) Go to the configuration > probe z offset menu. Move the Z offset into the negative range until it start to grip the paper
5) Save the settings by clicking configuration > store settings.

### Live-Adjusting the Probe Z Offset

You can now adjust the offset on the fly! This is really useful for getting just the right first layer 'squish'. There are two ways of doing this: 

1) While printing, click the select button four times quickly.
2) While printing, go to configuration or tune, then probe z offset

** SAVE the setting with Store Settings to make the setting stick! 

## Installation Procedure: 

XLoader is a program designed to upload firmwares to your 3d printer. Download XLoader from this source: http://www.hobbytronics.co.uk/arduino-xloader

1) Plug your printer into your computer
2) Open XLoader. Configure it with the following values: 
      - Hex File: Please download the "Cr20 Pro 3DPC Update.hex" from this repository
      - Device: MEGA(ATMEGA2560)
      - COM Port: The com port for your printer (should only be 1-2 there - try both if you don't have success at first)
      - Baud Rate: 115200
3) Press Upload.
