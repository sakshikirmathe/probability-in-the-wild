# Project 2: Customer Churn Analysis Using Bayesian Thinking

## Overview
Customer churn is a critical business problem, but raw churn rates alone provide
limited insight into *why* customers leave.

This project analyzes customer churn using **probability and conditional probability**,
treating churn likelihood as a **belief that updates as new customer information is observed**.
The analysis focuses on **Bayesian intuition**, not mathematical derivations or predictive models.

---

## Objectives
- Establish a baseline (prior) probability of customer churn
- Analyze how different customer attributes update churn belief
- Compare the strength of individual churn signals
- Understand how multiple risk factors compound churn probability

---

## Key Questions Explored
- What is the overall probability that a customer churns?
- How does churn probability change based on:
  - contract type?
  - availability of technical support?
- How does churn risk change when multiple risk factors are present?
- Which factor provides the strongest signal of customer churn?

---

## Bayesian Perspective
Churn probability is treated as a **belief**:

- **Prior belief**: Overall churn rate across all customers
- **Evidence**: Customer attributes such as contract type and service support
- **Updated belief**: Churn probability conditioned on observed evidence

This mirrors real-world decision-making, where beliefs are continuously updated
as new information becomes available.

---

## Key Insights
- Customers on **month-to-month contracts** have significantly higher churn risk
  compared to those on long-term contracts.
- Lack of **technical support** is a strong independent churn signal.
- Observing **multiple risk factors together** (month-to-month contract + no tech support)
  results in the largest increase in churn probability.
- Combined evidence provides a stronger belief update than any single signal alone.

---

## Tools Used
- Python
- Pandas
- NumPy

---

## Learning Focus
This project intentionally avoids machine learning models.

The emphasis is on:
- Probabilistic reasoning
- Bayesian belief updating
- Interpreting customer behavior through conditional probability
- Communicating insights in a business-relevant manner

These skills are directly applicable to analytics, data science,
and product-focused roles.
