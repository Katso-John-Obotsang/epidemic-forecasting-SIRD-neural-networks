# Epidemic Forecasting using SIRD and Neural Networks

### Mechanistic Epidemic Modeling, Neural Forecasting, and Robustness Analysis

---

## Abstract

Epidemic forecasting plays a critical role in public health planning, outbreak monitoring, and healthcare resource allocation. Traditional epidemiological models provide interpretable mathematical descriptions of disease spread, while machine learning models offer flexible data-driven forecasting capabilities.

This project investigates epidemic forecasting using both a classical **SIRD (Susceptible–Infected–Recovered–Deceased)** compartmental model and **Neural Network-based time-series forecasting**. The study compares mechanistic and data-driven approaches, evaluates forecasting performance, and analyzes robustness under noisy epidemic conditions.

The project further explores recursive future forecasting and demonstrates how neural forecasting models may become unstable when uncertainty and reporting noise are introduced into epidemic data.

---

## 1. Problem Statement

Epidemic forecasting systems face several important challenges:

* Capturing nonlinear epidemic dynamics accurately
* Maintaining interpretability in forecasting systems
* Forecasting future trajectories under uncertainty
* Handling noisy and irregular epidemic data
* Balancing mechanistic modeling with data-driven learning

This project addresses these challenges by combining differential equation-based epidemic modeling with neural network forecasting approaches.

---

## 2. Objectives

* Develop a classical SIRD epidemic simulation model
* Analyze parameter sensitivity in epidemic dynamics
* Generate synthetic epidemic time-series datasets
* Train neural networks for epidemic forecasting
* Compare mechanistic and data-driven forecasting approaches
* Investigate recursive forecasting behavior
* Evaluate robustness under noisy epidemic conditions

---

## 3. Mathematical Background

### 3.1 SIRD Model

The epidemic dynamics are governed by the following differential equations:

```math
dS/dt = -βSI/N

dI/dt = βSI/N - γI - μI

dR/dt = γI

dD/dt = μI
