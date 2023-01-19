# 32-Band-Audio-Visualizer

A 32 Band Audio Visualizer using FFT based around the ATMega328p

# Hardware

* 1x Any Arduino based around the ATMega328p, preferably a nano

* 1x 10k resistor

* 2x 100k resistor

* 3x 5k resistor

* 2x 100nf ceramic capacitors

* 1x push button

* 1x 8x32 MAX7219 dot matrix

* 1x TRS/TRRS audio jack

* 1x 5v PSU

# Schematics

   ![alt text](https://github.com/mzashh/32-Band-Audio-Visualizer/blob/main/schematics/schematics.png?raw=true)


*  For people using a Promini you will have to solder a wire to the AREF pin on the IC, refer to the following picture:

   ![alt text](https://github.com/mzashh/32-Band-Audio-Visualizer/blob/main/schematics/arefpromini.png?raw=true)
 
* Also the Promini has no 3.3v onboard, so you will have to use a voltage divider or a voltage regulator to generate it refer to the following picture:

   ![alt text](https://github.com/mzashh/32-Band-Audio-Visualizer/blob/main/schematics/voltagedivider.jpg?raw=true)

# Software

* Required libraries

   https://github.com/MajicDesigns/MD_MAX72XX

   https://github.com/kosme/arduinoFFT

* Method 1: Compiling the Arduino sketch and flashing it to the microcontroller.

* Method 2(not recommended): Flashing the precompiled hex file with xLoader.
 
   This method is not recommended as, parameters like Audio Response can't be fine tuned.

   https://github.com/binaryupdates/xLoader

