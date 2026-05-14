# Franchise vs. Original Film Forecasting Findings

## Background

One of the major design decisions in this project was whether sequel and franchise films should be included in the prediction target.

Initially, sequels were excluded from the target prediction set because franchise films appeared to introduce strong inherited signals that are unavailable to original films. However, franchise movies were still retained in the dataset for contextual feature engineering purposes, including:

- local competition density,
- release window saturation,
- semantic competition calculations,
- and market environment measurements.

The goal was to create a forecasting environment that better isolates the behavior of original films rather than allowing the model to heavily rely on pre-existing franchise awareness.

---

# Experimental Findings

## 1. Franchise Membership Is Extremely Predictive

Adding a simple franchise indicator column produced an approximately:

- **+0.03 increase in R²**
across nearly all model configurations.

This was one of the largest single-feature improvements observed during experimentation.

This suggests that franchise membership acts as a powerful prior for opening weekend performance.

---

## 2. Removing Franchise Films Significantly Increased Difficulty

When all franchise films were removed from the prediction target:

- dataset size dropped to approximately **1,493 movies**
- model performance dropped by roughly:
  - **~0.15 R²**

This indicates that forecasting original films is substantially harder than forecasting franchise films.



As a result, the forecasting problem becomes far noisier and more dependent on other features.

---

## 3. Franchise-Only Prediction Was Also Difficult

Interestingly, training only on franchise films also resulted in a noticeable performance drop:

- approximately **~0.10 R²**

This suggests that franchise forecasting is not inherently "easy" once franchise membership itself is no longer a separating signal.

Instead, the model must solve a more difficult problem:

> Why do some franchises open at \$40M while others open at \$200M?

This likely depends on:

- franchise strength,
- installment quality,
- audience fatigue,
- nostalgia effects,
- and semantic continuity between entries.

---

# Interpretation

These experiments suggest that movie box office forecasting may not represent a single homogeneous prediction problem.

Instead, the data appears to contain multiple forecasting regimes:

| Regime | Dominant Signals |
|---|---|
| Franchise Films | Brand equity, audience memory, franchise momentum |
| Original Films | Semantic positioning, novelty, market competition |

This distinction became especially important during semantic embedding experiments.

Dynamic entity embeddings and semantic identity features appear conceptually better aligned with original film forecasting, where audience perception and premise interpretation likely matter more.

---

# Project Direction

Based on these findings, the project will continue emphasizing:

- forecasting original films,
- retaining franchise films only for contextual calculations,
- and developing semantic representation features capable of capturing:
  - audience perception,
  - and evolving creative identities over time.

The franchise comparison experiments remain important because they demonstrate how strongly inherited IP structure affects predictive performance.

These findings also support the broader hypothesis that:
> movie forecasting performance is heavily influenced by the degree of pre-existing audience memory attached to a film.