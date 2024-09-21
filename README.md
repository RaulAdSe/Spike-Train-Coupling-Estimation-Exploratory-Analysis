# Spike Train Coupling Estimation: Exploratory Analysis

This repository contains an exploratory analysis of spike train data, with a focus on estimating the coupling strength \( \epsilon_2 \) between spike trains using different probability estimators: **Maximum Likelihood (ML)** and **Krichevsky-Trofimov (KT)**. The project investigates how these estimators behave under different conditions, such as varying firing rates, spike train lengths, and coupling strengths.

## **Contents**

- `Spike Train Generation.ipynb`: Jupyter notebook for generating spike trains with different firing rates and coupling strengths.
- `Probability_estimators.ipynb`: Jupyter notebook implementing the ML and KT probability estimators.
- `README.md`: Project documentation.
- `requirements.txt`: List of Python libraries required to run the project.

## **Project Overview**

### **Goal**

The primary goal of this project is to explore the behavior and accuracy of two probability estimation methods, **ML** and **KT**, when estimating the coupling strength \( \epsilon_2 \) between two spike trains. Spike trains are generated with different parameters such as firing rate, spike train length, and true coupling strength, and the performance of the estimators is compared across these conditions.

### **Key Concepts**

- **Coupling Strength (\( \epsilon_2 \))**: Represents the probability that a spike in train \( Y \) follows a spike in train \( X \).
- **ML Estimator**: A straightforward estimator based on counting occurrences and probabilities.
- **KT Estimator**: A Bayesian-like estimator designed to handle small datasets or sparse data, providing smoother estimates.

### **Structure**

1. **Spike Train Generation**:
   - Spike trains \( X \) and \( Y \) are generated with a fixed firing rate for \( X \) and a coupling probability \( \epsilon_2 \) governing \( Y \)'s behavior based on \( X \).
   
2. **Estimation Methods**:
   - **Maximum Likelihood (ML)**: Calculates \( \epsilon_2 \) directly from observed data.
   - **Krichevsky-Trofimov (KT)**: A probabilistic estimator that smooths the estimates, especially useful for small sample sizes.
   
3. **Exploratory Analysis**:
   - **Study 1**: Performance of estimators as a function of coupling strength.
   - **Study 2**: Analysis of \( \epsilon_2 \) estimation as a function of spike train length.
   - **Study 3**: Comparison of ML and KT estimators under different firing rates.
   - **Study 4**: Parameter tunning to find a case where KT is better than ML.

### 
