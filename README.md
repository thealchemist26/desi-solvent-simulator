DESI Solvent Flow Simulator
Overview
This Python application simulates the Desorption Electrospray Ionization (DESI) solvent flow over various fingerprint ridge patterns using the Lattice Boltzmann Method (LBM). It provides a graphical user interface (GUI) for users to adjust simulation parameters and visualize the solvent flow in real-time.

Features
Interactive GUI: Allows users to adjust various parameters of the DESI setup and fingerprint surface.

Real-time Visualization: Displays the solvent flow over the fingerprint surface as it evolves over time.

Multiple Ridge Patterns: Supports different fingerprint ridge patterns including parallel lines, wavy lines, and whorls.

Adjustable Parameters: Users can modify spray angle, tip-to-surface distance, spray width, and more.

DESI Schematic: Provides a visual representation of the DESI emitter setup.

Dependencies
NumPy

Matplotlib

PIL (Python Imaging Library)

Tkinter

SciPy

Installation
Ensure you have Python 3.x installed on your system.

Install the required dependencies:

bash
pip install numpy matplotlib pillow scipy
Download the script file.

Usage
Run the script:

bash
python desi_solvent_flow_simulator.py
The main application window and a schematic window will appear.

Adjust the simulation parameters using the sliders and dropdown menus.

Click "Initialize Simulation" to start or reset the simulation.

Use the "Flow Time Step" slider to advance the simulation and observe the flow patterns.

Key Components
Simulation Parameters
Fingerprint Ridge Type: Choose between parallel lines, wavy lines, or whorl patterns.

Ridge Pattern Rotation Angle: Rotate the ridge pattern (-180° to 180°).

DESI Sprayer Angle: Adjust the angle of the solvent spray (1° to 179°).

Tip to Surface Distance: Set the distance between the DESI tip and the surface (1mm to 10mm).

Spray Width Factor: Modify the width of the spray (0.5 to 2.0).

Spray Profile Type: Select between Gaussian or uniform spray profiles.

Wetting Factor: Adjust the surface wetting properties (0.0 to 1.0).

Visualization
The main window displays a color-coded representation of the solvent flow velocity.

Optionally show ridge patterns overlaid on the flow visualization.

A separate window shows a schematic of the DESI emitter setup.

Simulation Control
Initialize or reset the simulation with current parameters.

Control the progression of the simulation using the time step slider.

Lattice Boltzmann Method (LBM) Implementation
The simulation uses the D2Q9 LBM model:

2D grid (300x100)

9 velocity directions

Relaxation time (tau) set to 1.0

Collision and streaming steps implemented for fluid dynamics

Limitations and Future Improvements
The current wetting model is simplified and could be enhanced for more accurate surface interactions.

Performance optimizations may be needed for larger simulations or real-time adjustments.

Additional ridge patterns or custom pattern import could be implemented.

Contributing
Contributions to improve the simulation accuracy, add features, or optimize performance are welcome. Please submit pull requests or open issues for any bugs or suggestions.

[![Python Version](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Documentation Status](https://img.shields.io/badge/Documentation-Complete-brightgreen.svg)](README.md)

![image](https://github.com/user-attachments/assets/40f89678-04b9-47ce-8064-14e8088ffd4e)

![image](https://github.com/user-attachments/assets/3dd7ae1b-4872-427f-9586-7cfdd34fd52e)
