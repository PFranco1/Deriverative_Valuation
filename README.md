README
This repository provides various Python methods for pricing European and American-style derivative contracts. This is code adapted from Python for Finance, 2nd ed. by Dr. Yves J. Hilpisch, with additional functionality for fetching real-time option prices.

Purpose
These files aim to inform investors and researchers about estimating the fair value of options under both European and American exercise features. Please note that this code is for educational and informational purposes only and does not constitute financial advice.

American Option Valuation (Longstaff–Schwartz Method)
The American-style option valuation implemented here follows the Longstaff–Schwartz Monte Carlo (LSM) algorithm:

Well-Established Standard

Introduced by Longstaff and Schwartz (2001), LSM is a widely used, canonical approach for pricing American options by simulating possible price paths and determining the optimal early-exercise strategy.
Discrete-Time Approximation

As with most Monte Carlo methods, time is discretized. While this means true continuous exercise cannot be captured exactly, a sufficiently dense time grid typically provides a close approximation.
Regression-Based Continuation Values

LSM uses polynomial regression to estimate the option’s continuation value at each step. The accuracy of the method depends on the chosen number and type of basis functions.
Sufficient Simulation Paths

For reliable valuations, it is crucial to have a large number of simulated paths and a reasonable time step granularity.
Conclusion
With a proper choice of simulation paths, time steps, and basis functions, the LSM approach offers a robust and widely accepted technique for pricing American-style options, including certain path-dependent payoffs.

Disclaimer: Use this code at your own risk. It does not constitute investment advice. Always perform independent due diligence or consult with a qualified professional before making any financial decisions.
