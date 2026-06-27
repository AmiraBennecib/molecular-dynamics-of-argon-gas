# 2D Lennard-Jones Molecular Dynamics Simulation

A molecular dynamics simulation of a 2D Lennard-Jones fluid, implemented from scratch in Python using the Störmer-Verlet integrator in the microcanonical (NVE) ensemble.

## Overview

This project simulates N=25 argon-like particles interacting via the Lennard-Jones pair potential in a 2D periodic box. It was developed as a computational physics portfolio project to explore classical statistical mechanics through numerical simulation.

## Physics

The Lennard-Jones potential:

$$U(r) = 4\varepsilon \left[ \left(\frac{\sigma}{r}\right)^{12} - \left(\frac{\sigma}{r}\right)^{6} \right]$$

All quantities are expressed in **LJ reduced units** (ε=1, σ=1, m=1).

| Parameter | Value |
|-----------|-------|
| N (particles) | 25 |
| ρ (density) | 0.8 σ⁻² |
| dt (time step) | 0.005 τ |
| Time steps | 5000 |
| Ensemble | NVE (microcanonical) |

## Results

- **Energy conservation**
- **RDF**: liquid-like structure with first peak near r ≈ 1.1 σ
- **MSD**: linear growth in the diffusive regime — D ≈ 0.06 (LJ units)
- **Velocity distribution**: Gaussian vx and Rayleigh speed distribution, consistent with Maxwell-Boltzmann statistics


## Files

- `argon-md.ipynb` — main simulation notebook 

## Implementation of Lab Problem 12

This code is my own implementation of the **Maxwell Distribution** simulation from:

**Lectures on Computational Physics**  
Badis Ydri, Adel Bouchareb, Rafik Chemam  
Physics Department, Badji Mokhtar University, Annaba, Algeria  
May 21, 2013

**Lab Problem 12: Maxwell Distribution** (Section 7.5)

### Reference
- PDF: https://www.google.com/url?sa=t&source=web&rct=j&opi=89978449&url=https://homepages.dias.ie/ydri/COMPUTATIONALNOTES_FINAL.pdf&ved=2ahUKEwjdy8nwwKeVAxU8_7sIHV6vAPkQFnoECCMQAQ&usg=AOvVaw0QRLmbd2vD_wpaqQDxUDU1
- Original authors: Badis Ydri et al.
