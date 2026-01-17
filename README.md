# Directional Surface Wear via Tangent Flow Fields

This repository accompanies a short technical note exploring a minimal method for generating directional (anisotropic) surface wear on polygonal meshes using geometry-derived flow fields in Houdini.

The goal of this project is not to simulate physically accurate erosion, but to investigate whether directional wear patterns can be produced using simple surface-aligned vector fields derived from curvature and normal information.

## Contents

- `paper/`  
  The full technical note describing the method, math, and observations.

- `hip/`  
  Houdini scene files demonstrating the approach on simple and complex geometry.

- `images/`  
  Visual results and flow field visualizations.

- `cops/`  
  Screenshots of the Copernicus networks used to generate wear maps.

- `code/`  
  VEX snippets used for flow field construction and surface advection.

## Overview

The method consists of:
1. Computing surface curvature and normal information.
2. Constructing a tangent-space flow field by combining curvature gradients and normal-map detail.
3. Stabilizing the flow field to avoid sinks and surface collapse.
4. Applying directional surface advection driven by an artist-authored wear map.

This work is intended as a small, self-contained experiment and a foundation for further exploration.

## Software

- Houdini 21 (SOPs, SOP Solver, Copernicus)

## Author

Hrushikesh Dahiwaad

