# desi-solvent-simulator

# DESI Solvent Flow Simulator
A scientific simulation tool for modeling DESI (Desorption Electrospray Ionization) solvent flow patterns over surfaces using the Lattice Boltzmann method.

[![Python Version](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Documentation Status](https://img.shields.io/badge/Documentation-Complete-brightgreen.svg)](README.md)

## Overview
This simulator models the interaction between DESI solvent droplets and surfaces, allowing researchers to:

















The diagram above illustrates the key components of the DESI process that this simulator models. The electrospray emitter generates charged solvent droplets that interact with the surface, causing desorption of molecules. These molecules then undergo ionization and are analyzed by a mass spectrometer. The simulator focuses on modeling the interaction between the charged solvent droplets and the surface, which is crucial for optimizing DESI performance.

Let's look at how the simulator implements this process:














The simulation process shown above implements the Lattice Boltzmann method, where:

Streaming: Particles move to adjacent lattice cells according to their velocity directions
Collision: Particles at each cell interact and reach equilibrium based on local density and velocity
Update State: Macroscopic properties (density and velocity) are computed from the particle distribution
