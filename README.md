# Commodity-Pricing-Model
Implementation and comparison of three commodity pricing models: Schwartz One-Factor, Gibson-Schwartz Two-Factor, and Lucia-Schwartz seasonal model. Includes calibration to simulated data, path simulation, and comparative visualization of price dynamics.
Here's the clean content you can directly copy to your README.md file:

Commodity Derivative Pricing and Calibration

This project implements three commodity pricing models with calibration and simulation capabilities:

1. Schwartz One-Factor Model (1997)
- Models mean-reverting commodity prices
- d(ln St) = κ(μ - ln St)dt + σdWt
- Suitable for oil, metals and energy commodities

2. Gibson-Schwartz Two-Factor Model 
- Extends Schwartz model with stochastic convenience yield
- dSt = (r - δt)Stdt + σSStdWt
- dδt = κ(α - δt)dt + σδdWt
- Suitable for commodities with storage costs

3. Lucia-Schwartz Model (2002)
- Incorporates seasonal patterns with mean reversion  
- ln St = f(t) + Xt where f(t) is seasonal component
- dXt = κ(μ - Xt)dt + σdWt
- Suitable for agricultural commodities and natural gas

Features:
- Monte Carlo path simulation for each model
- Parameter calibration to market data
- Price calculation at maturity
- Comparative visualization of model behaviors

Installation:
1. Clone the repository
2. Install requirements: pip install numpy scipy matplotlib

Usage:
- Run main.py to execute the complete analysis
- The script will:
  - Calibrate each model to synthetic data
  - Simulate price paths
  - Calculate expected prices
  - Generate comparative plots

Output Includes:
- Calibrated parameters for each model
- Expected commodity prices at maturity
- Visualization comparing simulated paths

Note on Calibration:
The calibration demonstrates basic functionality. For production use:
- More robust optimization may be needed
- Real market data should be used
- Additional diagnostics would be valuable

This implementation serves as an educational demonstration of commodity pricing models and their calibration processes.
