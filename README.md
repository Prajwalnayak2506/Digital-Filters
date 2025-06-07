# Digital Filter Design – EE338 DSP Project

This repository contains the implementation of multi-band IIR and FIR filters designed as part of the EE338 Digital Signal Processing course project. The filter specifications are based on the assigned filter number **M = 114**.

## 📌 Project Overview

The goal of the project was to design and analyze various types of digital filters using Python, without relying on high-level filter design commands. The focus was on:

- Accurate realization of IIR and FIR filters
- Adherence to given frequency bands and ripple tolerances
- Manual implementation of transformation and design logic
- Visualization and validation of frequency responses

## 🛠️ Filter Types Implemented

1. **Type 1 – IIR Multi-Bandpass Filter**  
   - Passbands from Group I & Group II (monotonic response)
   - Designed using Butterworth/Chebyshev approximation  
   - Implemented with bilinear and frequency transformations

2. **Type 2 – IIR Multi-Bandpass Filter**  
   - Passbands with equiripple behavior
   - Stopbands are monotonic
   - Designed using Chebyshev Type I / Type II techniques

3. **FIR Multi-Bandpass Filter (Kaiser Window)**  
   - Passbands from Group I & II  
   - Designed using Kaiser window with custom beta and order calculations  
   - Frequency response tailored to passband/stopband ripple constraints

## 🧮 Tools Used

- **Language:** Python  
- **Libraries:** NumPy, SciPy, Matplotlib  
- **Approach:** Manual computation of filter coefficients, frequency normalization, and custom visualization

## 📊 Validation

Each filter was verified by:
- Computing magnitude and phase response
- Ensuring passband magnitude lies in [0.85, 1.15]
- Confirming stopband magnitude lies below 0.15

