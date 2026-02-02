# Applied Metrics – Problem Set 03  
## Causal Inference with Directed Acyclic Graphs (DAGs)

This repository contains the solutions to **Problem Set 03** of the *Applied Metrics (MSc)* course (Spring 2025).  
The project focuses on **causal inference**, **Directed Acyclic Graphs (DAGs)**, correct control variable selection, and bias arising from incorrect model specification.

---

## Files

- **causal-inference-dag-econometrics.ipynb**  
  Python notebook containing all analyses, DAG constructions, regressions, and explanations.

- **problem set 03.pdf**  
  Official problem set description.

---

## Problem Set Overview

### Part 1 – Causal Analysis of Fast Food Consumption and Heart Disease

This part studies the causal effect of **fast food consumption** on **heart disease risk** using a DAG-based framework.

#### Tasks:
- Construction of a **Directed Acyclic Graph (DAG)** including:
  - Fast food consumption
  - Physical activity
  - Diet quality
  - BMI
  - Blood pressure
  - Age
  - Gender
  - Genetic risk
- Identification of:
  - **Confounders** that must be controlled
  - **Bad controls** (mediators and colliders) that should not be controlled

#### Regression Analysis:
Two regression specifications are estimated using simulated data:

1. **Full Specification**  
   Controls for all available variables:
   - Demonstrates over-control bias and conditioning on mediators.

2. **Correct Specification**  
   Controls only for the appropriate confounders based on the DAG.

The coefficient of fast food consumption is compared across models, and the **direction and magnitude of bias** in the full specification are discussed.

---

## Part 2 – DAG Construction for Causal Questions

DAGs are constructed for **four causal questions**, each including:

- A clear causal diagram
- Identification of at least one **confounder**
- Identification of at least one **mediator or collider** and explanation of why it should not be controlled

The selected topics are analyzed conceptually with emphasis on causal reasoning rather than estimation.

---

## Part 3 – Backdoor Path Identification

Using a provided causal diagram:

- All **backdoor paths** between variables \(X\) and \(Y\) are identified.
- Each backdoor path is explained in terms of how it may bias causal estimates.
- A **sufficient adjustment set** is determined based on the backdoor criterion.

This section emphasizes correct identification strategies in causal inference.

---

## Methods and Concepts Used

- Directed Acyclic Graphs (DAGs)
- Confounders, mediators, and colliders
- Backdoor criterion
- Omitted variable bias
- Over-control bias
- Regression comparison for bias assessment

---

## How to Run

1. Clone the repository:
   ```bash
   git clone <repository-url>
