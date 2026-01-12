# Spatial filtering, histogram matching, steganography, HDR

## Overview
This repository contains implementations, experiments, and analyses for spatial filtering, histogram matching, bit-plane steganography, and HDR merging/tone-mapping as required in Assignment 1. All filtering/processing code (except image I/O/display) is implemented from scratch in the Jupyter notebook.

## What I implemented
- **Spatial filtering**
  - Mean (average) filter with variable kernel sizes; visual comparisons showing blur vs noise reduction.
  - Gaussian filter implemented from a parameterized kernel (kernel size, σ).
  - Edge detectors: Prewitt, Sobel, Laplacian (implemented as convolution kernels).
  - Image sharpening: unsharp masking and high-boost filtering (parameter sweep for boost factors).
- **Histogram matching**
  - From-scratch histogram and CDF computation, and histogram matching for multi-channel images.
  - Visualizations: source, target, and matched images with per-channel histograms.
- **Steganography**
  - Extracted and visualized all 8 bit-planes to locate hidden information.
  - Implemented embedding and extraction functions for binary secrets (`encrypt` / `decrypt`).
  - Analysis on MSB vs LSB embedding choices.
- **HDR**
  - HDR merge using exposure-weighted combination.
  - Tone-mapping using log compression and gamma correction; comparison with inputs.  



Please refer to Notebook for more details: src/main.ipynb