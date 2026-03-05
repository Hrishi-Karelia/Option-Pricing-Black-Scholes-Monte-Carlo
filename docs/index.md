# Option Pricing using Black-Scholes Model and Monte Carlo Simulation

## Overview

This project implements the **Black-Scholes Model (BSM)** to price European call and put options and compute key **Option Greeks**.
It also uses **Monte Carlo Simulation** to model stock price movements and estimate option prices.

The goal of this project is to demonstrate how quantitative finance techniques can be implemented using **Python for financial modelling and risk analysis**.

---

## Model Parameters

| Parameter               | Value  |
| ----------------------- | ------ |
| Current Stock Price (S) | 100    |
| Strike Price (K)        | 100    |
| Time to Maturity (T)    | 1 Year |
| Risk-Free Rate (r)      | 5%     |
| Volatility (σ)          | 20%    |

---

## Black-Scholes Option Prices

| Option Type | Price |
| ----------- | ----- |
| Call Option | 10.45 |
| Put Option  | 5.57  |

These values are calculated using the **Black-Scholes analytical formula**.

---

## Option Greeks

| Greek | Value | Interpretation             |
| ----- | ----- | -------------------------- |
| Delta | 0.636 | Sensitivity to stock price |
| Gamma | 0.018 | Rate of change of Delta    |
| Vega  | 37.52 | Sensitivity to volatility  |
| Theta | -6.41 | Time decay of option value |

The Greeks help measure **risk exposure of an option position**.

---

## Call Option Price vs Stock Price

This graph shows how the **call option price increases as the underlying stock price rises**.

<img width="686" height="470" alt="948ed631-5e59-4ffa-a037-c2c5c90426d3" src="https://github.com/user-attachments/assets/4f88de6a-9134-4c77-8dc8-0db1ea649e1c" />


---

## Monte Carlo Stock Price Simulation

Monte Carlo simulation generates thousands of possible future price paths for the stock using **Geometric Brownian Motion**.

<img width="695" height="470" alt="b4c03f17-391c-4f55-90b3-4b109166833d" src="https://github.com/user-attachments/assets/beb8ab25-76f1-49e0-9e9c-5d3dffb4ee32" />


Simulation Parameters:

* Simulations: 1000
* Time Steps: 252 trading days

---

## Monte Carlo Option Pricing

| Method        | Call Price |
| ------------- | ---------- |
| Black-Scholes | 10.45      |
| Monte Carlo   | 10.38      |

Both methods produce **similar option prices**, validating the simulation model.

---

## Key Concepts Demonstrated

* Black-Scholes Option Pricing Model
* Option Greeks (Delta, Gamma, Vega, Theta)
* Monte Carlo Simulation
* Financial Risk Modelling
* Python for Quantitative Finance

---

## Technologies Used

* Python
* NumPy
* SciPy
* Matplotlib
* Jupyter Notebook

---

## Project Structure

```
Option-Pricing-Black-Scholes-Monte-Carlo
│
├── Project.ipynb
├── README.md
└── images
    ├── option_price_plot.png
    └── monte_carlo_paths.png
```

---

## Conclusion

This project demonstrates how **quantitative finance models can be implemented programmatically** to analyze option pricing and financial risk.
The combination of **analytical models (BSM) and simulation techniques (Monte Carlo)** provides a robust framework for financial analysis.

---
