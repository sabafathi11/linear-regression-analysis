# Regression Stability Study

This repository contains an analytical and experimental study of linear and nonlinear regression methods with a focus on **numerical stability**, **collinearity**, and **optimization techniques**.  
The project evaluates how different algorithms behave under well-conditioned and ill-conditioned data and examines the impact of model complexity on performance and overfitting.

---

## 📘 Project Overview

The study explores three main dimensions:

### 🔹 1. Numerical Methods for Linear Regression
We compare:
- **Normal Equations**
- **Singular Value Decomposition (SVD)**

Key goal: assessing performance differences in small datasets and in the presence of **severe collinearity**.

---

### 🔹 2. Optimization-Based Methods
We evaluate:
- **Batch Gradient Descent (BGD)**
- **Stochastic Gradient Descent (SGD)**

The analysis highlights:
- convergence behavior,
- runtime per iteration,
- scalability considerations,

---

### 🔹 3. Nonlinear Regression Models
We extend the regression model using **degree-2 polynomial features** and examine:
- improved fitting performance,
- decreased cost values,
- increased risk of overfitting and how to control it.

---

## 📊 Key Findings

- For small, well-conditioned datasets, **Normal Equations and SVD produce nearly identical results**.  
- Under strong collinearity, **SVD demonstrates superior numerical stability** and provides more reliable coefficient estimates.  
- **SGD scales better** for large datasets, but in small datasets used here, **BGD showed slightly lower per-iteration cost** due to reduced randomness.  
- Polynomial regression improves fit but must be monitored to avoid **overfitting**.

---

## 📁 Repository Structure

