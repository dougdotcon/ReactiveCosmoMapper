# ReactiveCosmoMapper 🌌

![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Expansion_Phase-purple.svg)
![Physics](https://img.shields.io/badge/Physics-Entropic%20Gravity-orange.svg)
![Validation](https://img.shields.io/badge/Validation-Bulletproof-brightgreen.svg)

## Abstract

The **ReactiveCosmoMapper** is a computational engine designed to verify the **Entropic Gravity** hypothesis (Erik Verlinde) against observational data. It operates on the premise that Dark Matter is not a particle, but an emergent geometric response of spacetime entropy to baryonic matter and cosmic expansion. This project successfully implements a pipeline that ingests raw astronomical data, applies the entropic interpolation kernel, and validates the model against:
1.  **Galactic Rotation Curves** (SPARC)
2.  **Large-Scale Structure Clustering** (SDSS)
3.  **Weak Lensing Tomography** (Phantom Potential)
4.  **Primordial Galaxy Formation** (JWST High-z)

## 1. Data Ingestion Pipeline

The system is built on a "Code-First Physics" approach, rejecting pre-processed catalogs that assume the $\Lambda$CDM model.

*   **SPARC (Galactic):** Converts Luminosity (3.6 $\mu m$) to Baryonic Mass ($M_{bar}$).
*   **SDSS (Cosmological):** Parallel ingestion of 50,000 galaxies ($z < 0.2$) for 3D mapping.

## 2. The Reactive Physics Kernel

The core engine (`src/reactive_gravity.py`) replaces the Newtonian Potential with the Entropic Interpolation formula:

$$ g_{obs} = \frac{g_N + \sqrt{g_N^2 + 4 g_N a_0}}{2} $$

Where $a_0 \approx 1.2 \times 10^{-10} m/s^2$ is the acceleration scale associated with the Hubble Horizon.

## 3. Validation Results (Phase 1: Foundations)

### 3.1 Galactic Dynamics (Rotation Curves)
We simulated **NGC 0024** using only baryonic mass. The model predicts the observed flat rotation velocity without Dark Matter.

![Rotation Curve Validation](Validation/NGC0024_rotation.png)

### 3.2 Cosmological Statistics (The "Turing Test")
We calculated the **Two-Point Correlation Function** $\xi(r)$ for 50,000 galaxies using a Geometry-Aware Random Catalog (correcting for $n(z)$).

![Statistical Validation](Validation/correlation_function_analysis.png)
*Result: The Entropic Universe matches the Power Law slope ($\gamma \approx 1.8$) and amplitude of the Standard Model.*

## 4. Expansion Results (Phase 2: Stress Testing)

### 4.1 Weak Lensing Tomography
We projected the 3D Entropic Potential into a 2D Convergence Map ($\kappa$).
*   **Left:** Newtonian Gravity (Baryons only) - Too weak to lens light.
*   **Right:** Reactive Gravity - **Phantom Mass** emerges spontaneously, creating the "Lensing Signal" usually attributed to Dark Matter halos.

![Lensing Map](Validation/lensing_prediction_map.png)

### 4.2 The "Impossible Galaxies" (JWST Crisis)
We simulated the collapse of a primordial gas cloud ($10^{10} M_{\odot}$) starting at $z=15$.
*   **Mechanism:** In the past, $H(z)$ was higher, making the entropic acceleration $a_0(z)$ much stronger ("Turbo Gravity").
*   **Result:** The Reactive Cloud (Orange) collapses to form a galaxy **much faster** than the Standard CDM model (Black), explaining the mature galaxies found by JWST at $z > 10$.

![JWST Collapse](Validation/jwst_collapse_comparison.png)

## 5. 3D Visualization

The project maps the "Cosmic Web" by converting Redshift space to Cartesian coordinates and connecting gravitationally associated galaxies.

![Cosmic Web](Validation/reactive_universe_viz.png)

## 6. Installation and Usage

### Requirements
```bash
pip install numpy pandas astropy astroquery scipy matplotlib
```

### Reproducing Results

**1. Foundations (Rotation + Statistics)**
```bash
python src/run_ingestion.py
python src/reactive_cosmo_mapper.py
python src/run_statistics.py
```

**2. Expansion (Lensing + Early Universe)**
```bash
python src/run_lensing.py
python src/run_early_universe.py
```

## Credits

**Engineered by:** Douglas H. M. Fulber & ReactiveCosmoMapper Agent
**Paradigm:** Code-First Physics
**Theory:** Emergent Gravity / Erik Verlinde
