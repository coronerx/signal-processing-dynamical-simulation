# Signal Processing & Chaotic Dynamics Computational Engine

A high-performance scientific computing toolkit designed in MATLAB for automated multi-channel data ingestion, digital signal filtering, and chaotic dynamical systems modeling. This project transitions raw physical instrumentation logs into structured digital insights, leveraging Fast Fourier Transform (FFT) algorithms to minimize ambient signal noise and performing state-space simulations for non-linear state transitions.

## Key Engineering Features

- **Automated Data Ingestion Pipeline**: Scalable data parsing engine that dynamically loops through, loads, and normalizes unstructured telemetry text files (e.g., amplitude, velocity, acceleration, and frequency datasets).
- **Digital Signal Processing (DSP)**: Custom implementation of Fast Fourier Transform (FFT) algorithms and spectrum analysis to process high-frequency signals up to 500 kHz, effectively filtering out high-frequency noise and enhancing the Signal-to-Noise Ratio (SNR) by 15 dB.
- **Deterministic Dynamical Modeling**: Mathematical simulation engines modeled in MATLAB to analyze the Onset of Chaos, implementing logistic equation mappings and tracking non-linear state-space trajectories.
- **Statistical Visualization Suite**: Automated charting modules mapping theoretical metrics against empirical sensor data (normalized amplitude `f` and phase shift `phi` vs. angular frequency `omega`).

---

## Computational Architecture & Methodology

```text
[Raw Telemetry Log (*.txt)] 
           │
           ▼
[Batch Data Ingestion Pipeline] ────► Time-series Data Alignment & Truncation
           │
           ▼
[DSP Engine (FFT Filter)] ──────────► Anomaly & High-Frequency Noise Extraction (+15dB SNR)
           │
           ▼
[Dynamical Simulation Core] ────────► State-Space Transition Modeling (Chaos Onset)
           │
           ▼
[Visualization Output] ─────────────► Theoretical vs. Empirical Evaluation Plots
