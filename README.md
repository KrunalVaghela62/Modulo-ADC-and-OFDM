# Modulo-ADC-and-OFDM
Modulo & Clipped Signal Reconstruction Algorithms

This repository contains MATLAB implementations, simulations, and analysis for reconstructing signals that undergo clipping, modulo folding, or low-rate nonlinear ADC operations. The work explores algorithmic strategies inspired by compressed sensing, linear prediction, blind estimation, and time–frequency separation principles.

📌 Contents

B2R2 signal reconstruction using Projected Gradient Descent

Linear Prediction + Chebyshev filtering for clipped signals

Monte Carlo simulations for reconstruction error analysis

Modified linear prediction without prior knowledge of 
𝑁
𝜆
N
λ
	​


Exhaustive search–based folded-sample prediction

OFDM symbol detection from low-rate modulo ADC samples

Blind modulo ADC architecture using LMS filter adaptation

🔍 Key Contributions
1. B2R2-Based Reconstruction

Recovered heavily clipped and modulo-folded signals using the B2R2 (Beyond Bandwidth Reconstruction Recovery) algorithm implemented via Projected Gradient Descent, leveraging time–frequency separation for stable recovery.

2. Linear Prediction With Chebyshev Filtering

Implemented linear prediction enhanced by Chebyshev polynomial filtering to reconstruct clipped signals.
Conducted Monte Carlo simulations to study reconstruction error vs:

Oversampling factor (OF)

Clipping ratio

3. Modified Linear Prediction (No Prior 
𝑁
𝜆
N
λ
	​

)

Developed a modified linear prediction method that does not require prior knowledge of 
𝑁
𝜆
N
λ
	​

.
Contributions include:

An exhaustive search strategy to identify the first folded sample

A complementary estimator to recover 
𝑁
𝜆
N
λ
	​

 even in noisy conditions

4. OFDM Detection from Modulo ADC Outputs

Proposed a robust OFDM symbol detection method using outputs from a low-rate modulo ADC, designed to operate under:

Quantization noise

Folding nonlinearity

Resolution limits

Explored detection strategies that remain reliable despite nonlinear ADC distortions.

5. Blind Modulo ADC Architecture

Investigated a blind modulo ADC system that assumes no prior knowledge of input spectral properties.
Work includes:

FIR filter prediction using LMS adaptation

Strategies to prevent error propagation under noise

Validation via extensive MATLAB simulations

