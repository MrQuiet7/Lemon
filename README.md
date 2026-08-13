<p align="center">
  <img src="assets/banner.JPG" alt="‌banner" width="100%" />
</p>


# Lemon 🍋

### Stereo 20-LED VU Meter

> When life gives you a lemon, plug your music into it.

### Lemon is a compact stereo VU meter built around two LM3915N-1 LED bar-graph driver ICs.

### The design provides 10 LED levels for each stereo channel, giving a total of 20 LEDs. It is intended to be used as a standalone audio visualizer or integrated into an amplifier.

## Features

* Stereo audio level display
* 2× LM3915N-1
* 20× rectangular LEDs
* 10 levels per channel
* Independent sensitivity adjustment for left and right channels
* 3.5 mm stereo AUX input
* 3.5 mm stereo AUX output
* Adjustable DOT / BAR display mode
* 15–25 V DC supply
* Designed for integration into an audio amplifier
* Two-layer PCB with large GND copper zones

## Design

* Lemon is based on the LED VU meter circuit published by Elliott Sound Products.

* The original circuit uses an LM3915 to drive ten LEDs according to the level of an incoming audio signal. Lemon uses two identical sections for the left and right channels.

* Each channel has its own sensitivity adjustment, allowing the two VU meters to be calibrated independently.

## Signal Flow

* The audio signal is passed through the board while each stereo channel is sampled by its respective LM3915 section for visual level indication.

## Power

* Lemon is designed for a 15–25 V DC supply.

* The PCB uses a single positive supply and ground connection. The LED supply path and LM3915 supply path are separated on the board according to the original circuit.

* The EARTH connection is kept separate from the main GND plane through the original 10 Ω connection, allowing the board to be integrated into a larger amplifier system without unnecessarily tying the two together.

## PCB

### The PCB was designed in KiCad with a focus on:

* Clean stereo symmetry
* Short and organized signal paths
* Large GND copper zones
* Easy component identification
* Through-hole construction
* Simple integration into an amplifier enclosure

### The two rows of LEDs form the main visual element of the board, with the LM3915 circuits and adjustment controls positioned behind them.

* Components

### Quantity	Component
* 2	LM3915N-1
* 20	Rectangular LEDs
* 2	50 kΩ potentiometers
* 2	3.5 mm stereo TRS jacks
* 2	82 Ω / 0.5 W resistors
* 2	1.2 kΩ resistors
* 2	2.2 kΩ resistors
* 2	10 kΩ resistors
* 2	10 Ω resistors
* 4	100 nF capacitors

### Component values and quantities should be verified against the final schematic and BOM before assembly.

## Project Status

* The VU meter circuit is based on the design published by Elliott Sound Products.

* Lemon is an independent PCB implementation and stereo adaptation of the circuit, with a custom PCB layout, mechanical arrangement, and visual design.

## License

#### GNU General Public License v3.0
