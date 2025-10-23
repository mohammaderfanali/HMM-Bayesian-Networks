<div align="center">
  <img src="https://cdn.freebiesupply.com/logos/large/2x/sharif-logo-png-transparent.png" width="150" height="150" alt="Sharif University Logo">
  <br><br>
  <h1 align="center">Hidden Markov Models (HMM) & Bayesian Networks</h1>
</div>

---

### :dart: About This Project

This repository contains the implementation for Practical Assignment 3 of the **Artificial Intelligence** course (Spring 2025) at the Computer Engineering Department, Sharif University of Technology. This project, implemented in a Jupyter Notebook (`.ipynb`), covers two fundamental topics in probabilistic AI from scratch:

1.  **Hidden Markov Models (HMM):** For sequence modeling.
2.  **Bayesian Networks:** For inference under uncertainty.

---

## 🧬 Part 1: Hidden Markov Models (HMM)

In this section, an HMM model is implemented to analyze and predict DNA sequences. The goal is to identify the hidden states "Coding" vs. "NonCoding" based on the observed nucleotide sequence (A, C, G, T).

### Key Implementations:

* **:floppy_disk: Parameter Extraction (MLE):** Calculating the Initial, Transition, and Emission probabilities using Maximum Likelihood Estimation (MLE) from the labeled `dna_dataset.csv`.
* **:arrow_forward: Forward Algorithm:** Implementing the filtering algorithm to compute the probability of a specific observation sequence.
* **:v: Viterbi Algorithm:** Implementing the dynamic programming algorithm to find the single most likely sequence of hidden states that generated the observations.
* **:bar_chart: Visualization:** Plotting the Viterbi Path for visual analysis and validation of the model's predictions.

---

## 🕸️ Part 2: Bayesian Networks

In this section, four different inference algorithms are implemented and compared on a custom "Pizza Night" Bayesian Network. The objective is to compute conditional probabilities (e.g., the probability of 'High Satisfaction' given 'It's the Weekend').

### Implemented Inference Algorithms:

1.  **:mag: Exact Inference:**
    * **Enumeration:** A complete, recursive implementation that sums over all hidden variables.
    * **Variable Elimination (VE):** A more efficient exact algorithm that avoids redundant computations by using Factors, Join, and Eliminate operations.

2.  **:game_die: Approximate Inference:**
    * **Rejection Sampling:** A sampling method that generates samples from the prior distribution and rejects any sample that is inconsistent with the given evidence.
    * **Likelihood Weighting:** A more advanced sampling method that fixes the evidence variables and weighs each sample based on the likelihood of that evidence.

The notebook concludes with a comprehensive comparison of the accuracy and performance (runtime) of these four inference methods.

---

### :wrench: Tools & Technologies Used

* **Python 3**
* **Jupyter Notebook**
* **Pandas** (for managing the DNA dataset)
* **NumPy**
* **NetworkX** (for drawing the Bayesian Network structure)
* **Matplotlib** (for Viterbi path visualization)

---
### 👨‍💻 Author
* **Mohammadreza Monemian**
