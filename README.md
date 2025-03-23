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
   git clone https://github.com/yourusername/desi-solvent-flow-simulator.git
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

[MIT License](LICENSE)

Citations:
[1] https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/46779592/d78871be-320c-445d-9b81-68311cddc1c2/paste.txt

---
Answer from Perplexity: https://www.perplexity.ai/search/d428d73f-c51c-4bd5-8ddf-6ab7703d3ed9?utm_source=copy_output

[![Python Version](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Documentation Status](https://img.shields.io/badge/Documentation-Complete-brightgreen.svg)](README.md)

![image](https://github.com/user-attachments/assets/40f89678-04b9-47ce-8064-14e8088ffd4e)

![image](https://github.com/user-attachments/assets/3dd7ae1b-4872-427f-9586-7cfdd34fd52e)
