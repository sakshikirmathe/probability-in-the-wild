# Probability in the Wild

This repository documents my hands-on learning of **probability, conditional probability,
and Bayesian thinking** using real, customer-focused datasets.

The emphasis is not on heavy mathematics or machine learning models, but on
**developing correct intuition**, asking the right questions, and translating
probability into meaningful business insights.


## Why This Repository Exists

Probability is often taught through formulas and abstract examples, which makes it
difficult to understand how it is actually used in real-world data problems.

This repository focuses on:
- Understanding probability through **customer behavior**
- Learning when and why **conditional probability** is useful
- Applying **Bayesian thinking as belief updating**, not as a formula
- Building intuition that is directly applicable to analytics, product, and data science interviews

## Repository Structure

```
probability-in-the-wild/
├── project-1-customer-funnel/
├── project-2-customer-churn/
├── project-3-distributions/
└── README.md
```

Each project explores probability from a different perspective, while sharing
the same foundational concepts.

## Project Overview

### Project 1: Customer Purchase Funnel Analysis  
**(Conditional Probability over Actions)**

This project analyzes how purchase likelihood changes as users move through
different stages of an e-commerce funnel.

**Core question type:**  
> “Given that a user has already done X, how likely are they to do Y next?”

**What changes probability here:**
- User actions
- Funnel progression
- Behavioral stages (home → product → cart → checkout)

**Key ideas explored:**
- Overall vs conditional purchase probability
- Why raw averages are misleading
- How intent strengthens across funnel stages
- Why some metrics (e.g., time on page) are weak signals on their own

**Mental model:**  
> Probability evolves as **behavior unfolds over time**.

This type of reasoning is commonly used in:
- Product analytics
- Funnel optimization
- Growth analysis
- A/B test interpretation

### Project 2: Customer Churn Analysis Using Bayesian Thinking  
**(Belief Update over Customer Attributes)**

This project analyzes customer churn by treating probability as a **belief that updates**
as new information about a customer is observed.

**Core question type:**  
> “Given what I know about this customer, how likely are they to churn?”

**What changes probability here:**
- Customer attributes
- Contract structure
- Service quality indicators

**Key ideas explored:**
- Prior belief (baseline churn rate)
- Evidence-based belief updates
- Comparing strength of churn signals
- How multiple risk factors compound churn probability

**Mental model:**  
> Probability evolves as **new information is observed**.

This type of reasoning is commonly used in:
- Retention analysis
- Risk assessment
- Customer segmentation
- Decision-making under uncertainty


## How the Two Projects Differ (and When to Use Each)

Although both projects rely on the same probability foundations, they answer
**fundamentally different questions**.

| Aspect | Project 1 | Project 2 |
|------|----------|----------|
| Focus | User behavior | Customer attributes |
| Data structure | Sessions / journeys | One row per customer |
| Time aspect | Sequential | Static |
| Core concept | Conditional probability | Bayesian belief update |
| Probability answers | “What happens next?” | “What do I believe now?” |
| Typical use cases | Funnels, growth | Churn, risk, retention |


## Conditional Probability vs Bayesian Thinking (Clarified)

- **Conditional Probability** answers:
  > “Among cases where A is true, how often does B occur?”

  Example:
  - P(Purchase | Cart)
  - P(Churn | Month-to-month)

- **Bayesian Thinking** extends this by adding a belief narrative:
  > “I start with a baseline belief, observe new evidence, and update that belief.”

  Example:
  - Start with overall churn rate  
  - Observe contract type → update belief  
  - Observe tech support status → update belief again  

Importantly, these projects **do not use Naive Bayes models**.
They use conditional probability and Bayesian reasoning conceptually,
without assuming feature independence or building classifiers.

### Project 3: Understanding Distributions Through Customer Data  
**(Normal, Binomial, and Poisson Intuition)**

This project focuses on developing intuition for **probability distributions**
and understanding **when to use which distribution** based on the data-generating process.

Instead of assuming distributions, the project examines:
- the shape of real data,
- the assumptions behind common distributions,
- and how business constraints affect distribution choice.

**Key questions explored:**
- When is the normal distribution a reasonable approximation?
- Why are binary outcomes naturally modeled using a binomial distribution?
- How are event counts over time correctly modeled using a Poisson distribution?

**Distributions covered:**
- **Normal distribution** for continuous variables (e.g., customer charges)
- **Binomial distribution** for binary outcomes (e.g., churn)
- **Poisson distribution** for event counts over time (synthetic example)

**Mental model:**  
> The correct distribution depends on **how the data is generated**, not just on its appearance.

This type of reasoning is commonly used in:
- Experiment analysis
- Capacity planning
- Risk estimation
- Statistical modeling assumptions


## Tools Used
- Python
- Pandas
- NumPy
- Matplotlib

## Learning Philosophy

This repository intentionally avoids:
- Machine learning models
- Black-box predictions
- Formula-heavy derivations

Instead, it focuses on:
- Asking the right probability questions
- Understanding dependencies and evidence
- Interpreting results in plain, business-relevant language

The goal is to build intuition that is:
- Interview-ready
- Transferable across domains
- Grounded in real data scenarios

Together, these projects move from understanding variability (Day 1),
to conditional reasoning (Day 2), and finally to selecting appropriate
probabilistic models for uncertainty (Day 3).

## Key Takeaway

> **Probability is not just about numbers.  
It is about understanding how uncertainty changes when context or information changes.**

This repository reflects that mindset.
