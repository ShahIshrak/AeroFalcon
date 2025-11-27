## AERO-structural optimization for Flight And Lift-Constrained Optimization of Nonlinear twist 
AERO FALCON: A Low-fidelity aero-structural optimization framework for small UAV wings. Combines classical lifting-line theory with ML-based airfoil polars (NeuralFoil), incorporating Reynolds variation, sweep effects, and structural constraints. Optimizes spanwise twist distribution to maximize C_L/C_D ratio for early-stage wing design.

---

## Table of Contents
- [Features](#features)
- [Case Study](#case-study)
- [Results and Visualization](#results-and-visualization)
- [References](#references)
- [License](#license)
- [Citation](#citation)

---

## Features

- **Aerodynamic Modeling**: Prandtl lifting-line theory with vortex lattice method
- **ML-Enhanced Analysis**: NeuralFoil integration for Reynolds-dependent airfoil polars
- **Structural Constraints**: Torsion beam theory with material yield limits
- **Comprehensive Drag Model**: Induced, profile, viscous, and sweep-dependent drag
- **Multi-Parameter Optimization**: Spanwise twist and sweep distribution
- **Real-time Visualization**: 3D wing geometry and performance plots
- **Torque‑box torsion model** for structural feasibility
- **Nonlinear constrained optimization:**
  - ***Sequential Least Squares Programming (SLSQP)*** for primary Optimization Process involving Gradient Descent.
  - ***Genetic Algorithm (GA)*** In case, SLSQP fails due to poor gradients or local minima. GA uses global-search mechanism to find the best solution.
- Spanwise twist optimization under torsional limits
---

## Case Study
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

---

## Results and Visualization:
- Additional figures (not in the published paper) are available here:

- Figure 1: Summary and 3D wing visualization at 32 km/h
- Figure 2: 3D visualization of the Unoptimized and Optimized Wing at 32 km/h
- Figure 3: Aerodynamic characteristics (C_L, C_D, C_L/C_D vs AoA) at 32 km/h
- Figure 4–6: Equivalent results at 109 km/h

### At Cruise Velocity 32 km/h (8.89 m/s):

![Summary of Results at 32 km/h](https://github.com/ShahIshrak/AeroFalcon/blob/main/sample_results/Figure_1_v_8.89.png?raw=true)  
*Figure 1: Summary of Results Obtained (v=8.89 m/s).*

![3D Wing (Both unoptimized and optimized)](https://github.com/ShahIshrak/AeroFalcon/blob/main/sample_results/Figure_2_v_8.89.png?raw=true)  
*Figure 2: Visualization of the 3D wing (Both Unoptimized and Optimized).*

![Comparison of Aerodynamic Characteristics of the Unoptimized and the Optimized Wing](https://github.com/ShahIshrak/AeroFalcon/blob/main/sample_results/Figure_3_v_8.89.png?raw=true)
*Figure 3: Comparison of Aerodynamic Characteristics of the Unoptimized and the Optimized Wing (V = 32 km/h)*


### At Cruise Velocity 109 km/h (30.278 m/s):

![Summary of Results at 109 km/h](https://github.com/ShahIshrak/AeroFalcon/blob/main/sample_results/Figure_1_v_30.278.png?raw=true)  
*Figure 4: Summary of Results Obtained (v=30.278 m/s).*

![3D Wing (Both unoptimized and optimized)](https://github.com/ShahIshrak/AeroFalcon/blob/main/sample_results/Figure_2_v_30.278.png?raw=true)  
*Figure 5: Visualization of the 3D wing (Both Unoptimized and Optimized).*

![Comparison of Aerodynamic Characteristics of the Unoptimized and the Optimized Wing](https://github.com/ShahIshrak/AeroFalcon/blob/main/sample_results/Figure_3_v_30.278.png?raw=true)
*Figure 6: Comparison of Aerodynamic Characteristics of the Unoptimized and the Optimized Wing (V = 109 km/h)*

---

## References
[1] Asif Hasnayeen, Md Redwan Iqbal, Farhan Syeed and Morsalin Sheikh. "Construction of a Small Fixed Wing UAV for Surveillance," AIAA 2024-90565. 2024 Regional Student Conferences. January 2024.

[2] Y. Beju and J. Mandal, "Expanded polystyrene (EPS) geofoam: Preliminary characteristic evaluation," Procedia Engineering, vol. 189, pp. 239–246, 2017.


---

## License
- Apache License - See license file for more details.

## Citation
If you use AERO FALCON, please cite:

Md. Shah Ishrak, A Modular Framework for Low‑Fidelity Aero‑Structural Wing Twist Optimization of Small UAV Wings: AERO FALCON, ICMERE 2025.
