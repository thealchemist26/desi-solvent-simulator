# DESI Solvent Flow Simulator

## Overview

This Python application simulates the Desorption Electrospray Ionization (DESI) solvent flow over various fingerprint ridge patterns using the Lattice Boltzmann Method (LBM). It provides a graphical user interface (GUI) for users to adjust simulation parameters and visualize the solvent flow in real-time.

## Features

- Interactive GUI for adjusting DESI setup and fingerprint surface parameters
- Real-time visualization of solvent flow over the fingerprint surface
- Multiple ridge patterns: parallel lines, wavy lines, and whorls
- Adjustable parameters: spray angle, tip-to-surface distance, spray width, and more
- DESI schematic visualization
- Wetting factor control for surface interaction simulation

## Dependencies

- NumPy
- Matplotlib
- PIL (Python Imaging Library)
- Tkinter
- SciPy

## Installation

1. Ensure you have Python 3.x installed on your system.
2. Install the required dependencies:
   ```bash
   pip install numpy matplotlib pillow scipy
   ```
3. Clone this repository:
   ```bash
   git clone https://github.com/thealchemist26/desi-solvent-flow-simulator.git
   cd desi-solvent-flow-simulator
   ```

## Usage

Run the script:
```bash
python desi_solvent_flow_simulator.py
```

1. The main application window and a schematic window will appear.
2. Adjust the simulation parameters using the sliders and dropdown menus.
3. Click "Initialize Simulation" to start or reset the simulation.
4. Use the "Flow Time Step" slider to advance the simulation and observe the flow patterns.

## Key Components

### Simulation Parameters

- Fingerprint Ridge Type: Choose between parallel lines, wavy lines, or whorl patterns
- Ridge Pattern Rotation Angle: -180° to 180°
- DESI Sprayer Angle: 1° to 179°
- Tip to Surface Distance: 1mm to 10mm
- Spray Width Factor: 0.5 to 2.0
- Spray Profile Type: Gaussian or uniform
- Wetting Factor: 0.0 to 1.0

### Visualization

- Main window: Color-coded representation of solvent flow velocity
- Optional ridge pattern overlay
- Separate window: DESI emitter setup schematic

## Lattice Boltzmann Method (LBM) Implementation

- D2Q9 LBM model
- 2D grid (300x100)
- 9 velocity directions
- Relaxation time (tau) = 1.0
- Collision and streaming steps for fluid dynamics

## Limitations and Future Improvements

- Simplified wetting model
- Potential performance optimizations for larger simulations
- Opportunity for additional ridge patterns or custom pattern import

## Contributing

Contributions to improve the simulation accuracy, add features, or optimize performance are welcome. Please submit pull requests or open issues for any bugs or suggestions.

## License

[MIT License]

Copyright (c) 2025 Rohith Krishna

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

[![Python Version](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Documentation Status](https://img.shields.io/badge/Documentation-Complete-brightgreen.svg)](README.md)

Examples:

The GUI of the simulation software
![image](https://github.com/user-attachments/assets/40f89678-04b9-47ce-8064-14e8088ffd4e)

The simulation of DESI sovent flow over a whorl shape ridge pattern of fingerprint
![image](https://github.com/user-attachments/assets/3dd7ae1b-4872-427f-9586-7cfdd34fd52e)

The simulation of DESI sovent flow over a parallel shape ridge pattern of fingerprint
![image](https://github.com/user-attachments/assets/61ab198a-e542-471f-aa9f-a44ed9340696)

The simulation of DESI sovent flow over a arch shape ridge pattern of fingerprint

![image](https://github.com/user-attachments/assets/b7a174b8-3837-4200-86e7-4fbc0fdd141a)

The simulation of DESI sovent flow over a loop shape ridge pattern of fingerprint

![image](https://github.com/user-attachments/assets/6b4ba00f-9b41-4796-b9ed-e670ebb4084b)
