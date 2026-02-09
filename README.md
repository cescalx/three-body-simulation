# three-body-simulation
Three-body gravitational simulation with energy conservation and animation
# Three-Body Gravitational Simulation

This project implements a numerical simulation of a three-body gravitational system inspired by the Alpha Centauri binary star system with an orbiting planet.

The system is evolved using numerical integration of the equations of motion, with a small modification to the inverse-square gravitational force law. The simulation explores different orbital regimes (bound and unbound motion) and tracks energy conservation over time.

A 3D animation of the system is generated alongside diagnostic energy plots.

---

## Features

- Numerical integration of a three-body gravitational system
- Modified gravity with a small deviation from the inverse-square law
- Elliptic, near-parabolic, and hyperbolic orbital behaviour
- Energy diagnostics (kinetic, potential, total energy)
- 3D animated visualisation of orbital motion
- Output animation saved as a GIF

---

## Methods

The equations of motion are solved using SciPy’s ODE solvers.  
Positions and velocities of all bodies are evolved simultaneously in time.

Key physical elements:
- Newtonian gravity with a small power-law deviation
- Dimensionless rescaling of physical constants
- Vis-viva equation used to set initial orbital velocities
- Energy conservation used as a consistency check

---

## Visualisation

The simulation produces:
- A 3D animated orbit of the two stars and the planet
- Energy vs time plots showing kinetic, potential, and total energy

The animation below shows the evolution of the three-body system:

![Three-body animation](three_body_system_with_eccentricity0.5.gif)

---

## Technologies Used

- Python
- NumPy
- SciPy
- Matplotlib
- Jupyter Notebook

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/three-body-simulation.git
