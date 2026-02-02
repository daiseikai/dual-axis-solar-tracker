# dual-axis-solar-tracker
everything subject to change 

## What is it?
A dual-axis solar panel tracker that can aim at the brightest light source (demo mode) or follow the sun’s predicted position (solar position mode). Built for a desk-scale prototype using an Arduino, 2 servos, and light sensors.

## Modes/functionality
- 2-axis aiming (pan / tilt) using two servos
- Two tracking modes:
  1. Light Tracking (LDR mode): Uses multiple LDRs to center on the brightest light (mainly for indoor demo with a flashlight, but LDRs could be used to optimize solar mode). 
  2. Sun Position (Solar mode): Uses date/time and location from an RTC to compute where the sun should be, then points the panel accordingly. Especially useful on cloudy days.
- Night mode, where when the servos detect both light below a nighttime threshold and RTC gives a time generally post sunset, the panel will "park" (azimuth 0, elevation 0). This will save power. It will periodically check RTC and light levels in order to check when it should come back on

## Hardware
- Arduino Uno
- 2× SG90 micro servos
- 4× LDR photoresistors
- 10k resistors and 470 μF capacitor
- 2x 6V 60mA solar panels
- Breadboard and jumper wires
- 5V 2A Battery pack
- RTC

## Wiring
(to be updated)

## How to run
(to be updated)

