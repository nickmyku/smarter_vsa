# Smarter VSA

Intedned to be used on a 2008-2012 Honda Accord

The primary purpose of this system is to intelligentaly disable the car's VSA system and add mood lighting to the passenger cabin (because why not). Also lets add an unessasary OLED screen for good measure #FeatureCreep

No one likes VSA in fair weather, especially on a ~300hp front wheel drive coupe with an open differential, it completely criples the cars preformance. That being said if it did not have VSA during the winter months the car would be almost undrivable. This system will only disable the VSA if it is not raining (very humuid) and above freezing outside

## Hardware

There are four primary hardware components of the system:

* Adafruit Trinket Pro (5V/16MHz) [Product ID: 2000]
* SHT-10 Soil Temperature/Moisture Sensor [Product ID: 1298]
* Adafruit NeoPixel Stick [Product ID: 1426]
* Adafruit 128x64 OLED Display [Product ID: 938]

The code should run on most other arduino based platforms though

Other miscelleneous MOSFETs, voltage regulators, switches, diodes, resistors, and capacitors will be needed to fully recreate this project

## Notes

System stores all user definable values in EEPROM, which means they will be unintialized on a clean flash of the Trinket. Be sure to use the UI to save these values on first bootup or system could behave strangely.
