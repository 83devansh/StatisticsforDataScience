# Sunspot Analysis Using Gamma Distribution and MCMC

## Overview
This project analyzes monthly sunspot activity using historical data from the SILSO dataset. It includes data cleaning, visualization, Gamma distribution fitting, Markov Chain Monte Carlo (MCMC) sampling, parameter estimation, and simulation of future sunspot counts.

## Dataset
The data is collected from the **SILSO (Sunspot Index and Long-term Solar Observations)** dataset.

- Source: https://www.sidc.be/SILSO/DATA/SN_m_tot_V2.0.csv
- Time period: January 1749 to November 2018
- Total observations: 3,239 monthly records
- Target variable: Monthly Mean Sunspot Number

## Objectives
- Analyze historical monthly sunspot activity.
- Visualize sunspot variation over time.
- Divide the data into assumed 12-year cycles.
- Fit a Gamma distribution to sunspot counts.
- Perform MCMC sampling to estimate Gamma parameters.
- Visualize MCMC traces and posterior distributions.
- Estimate parameters with credible intervals.
- Simulate possible sunspot counts for the next 12 months.

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- SciPy

## Analysis Performed

### 1. Data Collection and Cleaning
Loaded the monthly sunspot dataset directly from the SILSO website, selected the required time period, and removed negative sunspot values.

### 2. Sunspot Activity Over Time
Created a line plot to observe the variation in sunspot numbers from 1749 to 2018 and identify repeated patterns of solar activity.

### 3. 12-Year Cycle Analysis
Assumed a solar cycle of 12 years (144 months) and assigned cycle numbers to the observations. Cycle boundaries were visualized using vertical lines.

### 4. Gamma Distribution Fitting
Fitted a Gamma distribution to positive sunspot counts to model their probability distribution.

### 5. Histogram Analysis
Created a histogram to examine the frequency distribution of monthly sunspot counts and understand their spread and skewness.

### 6. MCMC Sampling
Implemented a Metropolis-style MCMC algorithm with 30,000 iterations to estimate the Gamma distribution parameters:

- Initial shape parameter (a): 4
- Initial scale parameter (b): 10
- Burn-in samples: 5,000
- Proposal standard deviation: 0.12

### 7. Trace Plots and Posterior Distributions
Visualized the sampling chains for parameters `a` and `b` and plotted their histograms after removing burn-in samples.

### 8. Parameter Estimation
Calculated posterior means and 95% credible intervals for the Gamma parameters.

### 9. Simulation
Generated 12 simulated monthly sunspot counts using the estimated Gamma distribution parameters.

## Results

| Parameter | Estimated Value |
|---|---:|
| Shape (a) | 1.1733 |
| Scale (b) | 71.7167 |
| 95% CI for a | 1.1209 – 1.2238 |
| 95% CI for b | 67.9308 – 75.6814 |
| MCMC samples | 30,000 |
| Burn-in | 5,000 |

## Conclusion
The Gamma distribution provides a simple probabilistic model for positive sunspot counts. MCMC sampling was used to estimate the shape and scale parameters, and the posterior distributions were analyzed after removing burn-in samples.

The project also simulates 12 possible monthly sunspot counts based on the estimated parameters. These values represent probabilistic simulations and should not be considered an accurate time-series forecast because the model does not account for solar-cycle timing or temporal dependence.

## How to Run
1. Open the notebook in Google Colab or Jupyter Notebook.
2. Run the cells in sequence.
3. The dataset is downloaded automatically from the SILSO source.
4. Required libraries:

   ```bash
   pip install pandas numpy matplotlib scipy
   ```

## Future Improvements
- Use actual solar-cycle lengths instead of a fixed 12-year assumption.
- Compare Gamma with other probability distributions.
- Improve MCMC sampling and convergence diagnostics.
- Incorporate temporal dependence and solar-cycle patterns.
- Develop a proper time-series forecasting model.

