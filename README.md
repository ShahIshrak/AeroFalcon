# AERO FALCON 
## AERO-structural optimization for Flight And Lift-Constrained Optimization of Nonlinear twist 
AERO FALCON: A Low-fidelity aero-structural optimization framework for small UAV wings. Combines classical lifting-line theory with ML-based airfoil polars (NeuralFoil), incorporating Reynolds variation, sweep effects, and structural constraints. Optimizes spanwise twist distribution to maximize C_L/C_D ratio for early-stage wing design.

---

## Table of Contents
- [Features](#features)
- [Results and Visualization](#results-and-visualization)
- [Methodology](#methodology)
- [References](#references)
- [License](#license)

---

## Features

- **Aerodynamic Modeling**: Prandtl lifting-line theory with vortex lattice method
- **ML-Enhanced Analysis**: NeuralFoil integration for Reynolds-dependent airfoil polars
- **Structural Constraints**: Torsion beam theory with material yield limits
- **Comprehensive Drag Model**: Induced, profile, viscous, and sweep-dependent drag
- **Multi-Parameter Optimization**: Spanwise twist and sweep distribution
- **Real-time Visualization**: 3D wing geometry and performance plots

---

## Results and Visualization
The AERO FALCON framework has been demonstrated using a small fixed-wing UAV configuration based on Hasnayeen et al. [1]. 

### Wing Geometry
- **Airfoil**: Clark Y
- **Mean Aerodynamic Chord**: 0.21 m
- **Wingspan**: 1.28 m
- **Aspect Ratio**: 6.09
- **Wing Area**: 0.269 m²
- **Planform**: Rectangular

### Operating Conditions
- **Cruise Velocities**: 
  - Low-speed: 32 km/h (8.89 m/s)
  - High-speed: 109 km/h (30.278 m/s)
- **Altitude**: 1000 m
- **Aircraft Weight**: 1.8 kg (17.658 N)

### Structural Properties (EPS Foam [2])
- **Young's Modulus (E)**: 0.0038 GPa
- **Shear Yield Stress (τ_yield)**: 0.00509 MPa
- **Poisson's Ratio**: 0.15

## References
[1] A. Hasnayeen, M. R. Iqbal, F. Syeed, and M. Sheikh, "Construction of a Small Fixed Wing UAV for Surveillance," AIAA AVIATION Forum, 2024.

[2] Y. Beju and J. Mandal, "Expanded polystyrene (EPS) geofoam: Preliminary characteristic evaluation," Procedia Engineering, vol. 189, pp. 239–246, 2017.


---

## License
- Apache License - See license file for more details.
