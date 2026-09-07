# Kolam Euler Circuit LED Chaser

An Arduino-based NeoPixel LED chaser that traces the Euler circuit path of a traditional South Indian 
Kolam design — a geometric art form drawn daily with rice flour, which encodes mathematical concepts 
like Euler circuits, symmetry, and fractals.

**Full write-up (design context, math background, build photos):** [https://www.instructables.com/Your-Own-Flashing-Kolam-That-Traces-a-Euler-Circui]

## How it works

The Kolam pattern is mapped onto a sequence of NeoPixel LEDs following its Euler circuit — a path that 
traces every edge of the design exactly once, starting and ending at the same point. The Arduino Uno 
drives the LEDs in sequence along this path, lighting them up as a "chaser" that visually traces the 
circuit in real time.

## Hardware

- Arduino Uno
- WS2812B NeoPixel LEDs
- Square general-purpose PCB board (to mount the NeoPixels in the Kolam layout)
- Breadboard
- Soldering iron, flux, and solder
- 1000 µF, 25V capacitor
- 470 Ω resistor
- Jumper wires
- Arduino cable
- USB cable (one end cut and exposed, for breadboard power input)
- USB cable with a barrel jack soldered to the exposed end (for power input to the buck converter)
- XL4015 buck converter (stepped down to output 5V)
- Ambrane 20000mAh power bank (portable power source)

## Software / Libraries

- Written in Arduino C++
- Uses the Adafruit NeoPixel library

## Power setup

The circuit runs off a portable power bank stepped down through a buck converter to a steady 5V supply 
for the NeoPixels, making the whole build portable rather than tethered to a wall outlet.

## Wiring

Detailed wiring in the Instructables link provided at the top of the page
