# Project 1: Customer Purchase Funnel Analysis

## Overview
In customer-facing products, overall conversion rates are often low and can be misleading.
A more informative approach is to analyze **how purchase likelihood changes as customers
progress through different stages of the funnel**.

This project applies **probability and conditional probability** to understand customer
behavior across a purchase funnel, focusing on interpretation and decision-making rather
than predictive modeling.

---

## Objectives
- Apply basic probability concepts in a real business context
- Compute and interpret conditional probabilities across funnel stages
- Compare baseline purchase probability with stage-based probabilities
- Evaluate which customer signals provide the strongest indication of purchase intent

---

## Key Questions Explored
- What is the overall probability that a session results in a purchase?
- How does purchase probability change as users move through funnel stages?
- How does cart activity influence purchase likelihood?
- Does time spent on a page meaningfully increase purchase probability?
- Which single factor provides the strongest signal of purchase intent?

---

## Why Conditional Probability
Conditional probability answers questions of the form:

> “Given that a customer has already done **X**, how likely are they to do **Y**?”

In funnel-based products, this perspective is far more actionable than relying on
aggregate averages, as it reflects how user intent evolves with additional information.

---

## Key Insights
- Purchase probability increases sharply as sessions progress deeper into the funnel.
- Reaching later stages (cart and checkout) is a stronger signal of purchase than
  engagement metrics such as time spent on page.
- Adding the first item to the cart significantly increases purchase likelihood,
  while additional items provide diminishing signal.
- Time on page alone is not a reliable indicator of purchase intent when considered
  without contextual signals.

---

## Tools Used
- Python
- Pandas
- NumPy

---

## Learning Focus
This project intentionally avoids machine learning models.

The emphasis is on:
- Developing strong probabilistic intuition
- Understanding dependency between customer actions
- Translating statistical results into clear business insights

These skills are directly applicable to product analytics, growth analysis,
and data science interviews.