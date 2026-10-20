# Choosing Controls with Causal Graphs (DAGs)

A short applied study of how **directed acyclic graphs** guide the choice of control variables, and of the bias that comes from controlling for the wrong variables.

## Simulation: fast food and heart disease

A simulated population of 10,000 individuals, with a known causal structure linking fast-food consumption, exercise, diet quality, BMI, blood pressure, age, sex and genetic risk to heart disease.

- A DAG separates **confounders**, which must be controlled, from **mediators and colliders**, which must not
- Two regressions are compared: one controlling for everything available, one controlling only for the confounders the DAG identifies
- The coefficient on fast food changes between them. The gap is the over-control bias introduced by conditioning on mediators such as BMI and blood pressure

## Causal questions

DAGs are drawn for four further causal questions. Each identifies at least one confounder and at least one mediator or collider, and explains why conditioning on it would bias the estimate.

## Repository structure

```
causal-inference-dag-econometrics.ipynb   # simulation, regressions and DAGs
```

## Reproducing

```bash
pip install numpy pandas statsmodels
```

## Context

Developed during the MSc in Economics at Sharif University of Technology (Applied Econometrics, Spring 2025).

---
**Shayan Pourmasoomi** · MSc Economics, Sharif University of Technology · [LinkedIn](https://www.linkedin.com/in/shayan-pourmasoomi-8b6206389)
