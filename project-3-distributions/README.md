# Project 3: Understanding Distributions Through Customer Data

## Overview
This project explores **probability distributions** through real customer-related data
and a controlled synthetic example.

The goal is to develop intuition around:
- how different distributions behave,
- what assumptions they make,
- and when each distribution should be used in real-world analysis.

Rather than forcing data to fit a distribution, the project emphasizes
**examining the data-generating process first**.

---

## Distributions Covered

### Normal Distribution
Used to understand **continuous variables** and natural variation.

- Example: Monthly customer charges
- Focus:
  - Mean and standard deviation
  - Distribution shape
  - Why real business data often violates perfect normality

Key takeaway:
> Continuous data is not necessarily normally distributed, especially when shaped by business constraints such as pricing tiers.

---

### Binomial Distribution
Used for **binary outcomes** across a fixed number of trials.

- Example: Customer churn (Yes / No)
- Focus:
  - Fixed trials
  - Success / failure interpretation
  - Expected variation around average outcomes

Key takeaway:
> Binary customer outcomes across a fixed population naturally follow a binomial process.

---

### Poisson Distribution
Used for **event counts over time or space**.

- Example: Support tickets per hour (synthetic simulation)
- Focus:
  - Average event rate
  - Random arrival of events
  - Right-skewed distribution shape

Key takeaway:
> Poisson distributions model how often events occur, not how many attempts were made.

---

## Why This Project Matters
Choosing the wrong distribution can lead to:
- incorrect assumptions,
- misleading conclusions,
- and poor business decisions.

This project demonstrates that:
- distribution choice depends on **how data is generated**,
- visualization is essential for validating assumptions,
- and statistical intuition is as important as computation.

---

## Tools Used
- Python
- Pandas
- NumPy
- Matplotlib

---

## Learning Focus
This project avoids:
- distribution fitting for its own sake,
- formula-heavy derivations,
- and automated statistical tests.

Instead, it focuses on:
- intuition,
- interpretation,
- and correct reasoning about uncertainty.

---

## Key Takeaway
> **Distributions are models of uncertainty, not labels to be assigned blindly.**

Understanding their assumptions is essential for correct analysis.