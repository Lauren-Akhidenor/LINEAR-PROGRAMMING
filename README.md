# Optimising Agricultural Production Systems Using Linear Programming (Feed, Profit & Capacity Allocation)

*This project applies Linear Programming (LP) to real-world agricultural and agro-processing decisions, including feed formulation, production scheduling, and machine allocation. It demonstrates how constrained optimisation improves cost efficiency, profitability, and resource utilisation in small-scale food systems.*

[![📊 Linear Programming Optimisation ⚙️](https://img.shields.io/badge/GitHub-📊_Linear_Programming_⚙️-F5F5DC?logo=github&logoColor=white&labelColor=800020)](https://github.com/Lauren-Akhidenor/LINEAR-PROGRAMMING)

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Economic & LP Formulation](#economic--lp-formulation)
3. [Worksheet 1: Feed Formulation (Nutrient-Cost Optimisation)](#worksheet-1-feed-formulation-nutrient-cost-optimisation)
4. [Worksheet 2: Production Scheduling (Profit Maximisation)](#worksheet-2-production-scheduling-profit-maximisation)
5. [Worksheet 3: Machine Allocation Optimisation](#worksheet-3-machine-allocation-optimisation)
6. [Key Results Summary](#key-results-summary)
7. [Practical Applications](#practical-applications)
8. [Insights & Implications](#insights--implications)
9. [Limitations of the Model](#limitations-of-the-model)
10. [Executive Decision Insights (Managerial Summary)](#executive-decision-insights-managerial-summary)
11. [Summary](#summary)
---

## Project Overview
Linear Programming (LP) is a mathematical optimisation technique used to determine the best possible outcome (minimise cost or maximise profit) under resource constraints.

This project applies LP to three agricultural decision problems:

- **Feed formulation optimisation:** minimise cost while meeting nutrient requirements  
- **Production scheduling:** maximise profit from agro-processing activities  
- **Machine allocation:** optimise constrained processing time across products  

The results provide **decision-ready insights for farmers, feed millers, and small-scale processors**.

---

## Economic & LP Formulation

This study applies deterministic linear optimisation using Excel Solver.

### General LP Structure
- **Decision variables:** quantities of grains or products  
- **Objective function:** cost minimisation or profit maximisation  
- **Constraints:** nutrient requirements, machine capacity, production limits  
- **Non-negativity:** all variables ≥ 0  

---

## Worksheet 1: Feed Formulation (Nutrient-Cost Optimisation)

### Nutrient-Cost Optimisation
<details>
<summary>Click to expand Nutrient-Cost Charts</summary>
<img src="Screenshot (961).png" width="700">
</details>

### Real-world interpretation
Grains represent feed ingredients used in livestock ration formulation.

| Nutrient / Cost | Maize | Soybean Meal | Rice Bran | Requirement | Achieved |
|----------------|------|-------------|----------|------------|----------|
| Energy         | 20   | 30          | 70       | 110        | 110      |
| Protein        | 10   | 10          | 0        | 18         | 26.03    |
| Fibre          | 50   | 30          | 0        | 90         | 90       |
| Fat            | 6    | 2.5         | 10       | 14         | 14       |
| Cost (₦/kg)    | 41   | 36          | 96       |            | **148.61** |

### LP Model

**Objective:**
Minimise  
\[
Z = 41x₁ + 36x₂ + 96x₃
\]

**Subject to:**
- 20x₁ + 30x₂ + 70x₃ ≥ 110  
- 10x₁ + 10x₂ ≥ 18  
- 50x₁ + 30x₂ ≥ 90  
- 6x₁ + 2.5x₂ + 10x₃ ≥ 14  

**Optimal Solution:**
- Minimum cost = **₦148.61/kg**
- All nutrient constraints satisfied (Protein constraint shows slack → overachievement)

---

## Worksheet 2: Production Scheduling (Profit Maximisation)

### Maximised Profit
<details>
<summary>Click to expand Nutrient-Cost Charts</summary>
<img src="Screenshot (962).png" width="700">
</details>


### Decision context
A small agro-processing unit producing Maize Flour and Yam Flour under limited machine time.

### LP Model

Let:
- x₁ = Maize Flour output  
- x₂ = Yam Flour output  

**Objective:**
Maximise profit  
\[
Z = 2.25x₁ + 2.25x₂
\]
*(profit derived from solver output total = 270)*

**Subject to:**
- Machine I: 3x₁ + 2x₂ ≤ 300  
- Machine II: 2x₁ + 4x₂ ≤ 360  
- x₁, x₂ ≥ 0  

### Optimal Solution (Solver Result)
- x₁ = 60 units (Maize Flour)  
- x₂ = 60 units (Yam Flour)  
- **Maximum profit = 270**

### Interpretation
Both machines are fully utilised → **binding constraints**, meaning no idle capacity exists at optimum.

---

## Worksheet 3: Machine Allocation Optimisation

### Machine Allocation
<details>
<summary>Click to expand Machine Allocation Charts</summary>
<img src="Screenshot (964).png" width="700">
</details>



### Key finding: balanced allocation is optimal

| Maize Flour | Yam Flour | Machine Feasibility |
|------------|----------|---------------------|
| 60         | 60       | Fully feasible      |

### Optimal Outcome
- Optimal production mix: **60:60 (Maize:Yam)**
- Both Machine I and II constraints are exactly satisfied
- System operates at **full capacity efficiency**

### Interpretation
This represents a **corner solution**, where any deviation reduces feasibility or efficiency.

---

## Key Results Summary

| Worksheet | Objective | Optimal Result |
|----------|----------|---------------|
| WS1 | Minimise cost | ₦148.61/kg feed cost |
| WS2 | Maximise profit | 270 total profit |
| WS3 | Allocate machine time efficiently | 60:60 optimal mix |

---

## Practical Applications

### Feed Industry
- Enables precise least-cost ration formulation
- Identifies nutrient slack (e.g., Protein surplus → cost reduction opportunity)

### Agro-processing SMEs
- Confirms full machine utilisation at optimal solution
- Supports capacity expansion decisions

### Investment Insight
- Machine constraints are **binding bottlenecks**
- Expansion of either machine increases production capacity directly

---

## Insights & Implications

- LP transforms agricultural decision-making from heuristic to **mathematically optimal allocation**
- All three systems demonstrate **resource-constrained optimisation under scarcity**
- Results highlight the importance of:
  - constraint binding analysis
  - marginal capacity expansion decisions
  - cost efficiency in feed systems

---

## Limitations of the Model

While the Linear Programming framework provides clear optimisation insights, the following limitations should be acknowledged:

- **Deterministic assumptions:** All prices, machine capacities, and nutrient values are assumed constant, whereas real agricultural systems experience price volatility and supply fluctuations.

- **Linearity constraint:** The model assumes proportional relationships between inputs and outputs, ignoring potential non-linear effects such as economies of scale or diminishing returns.

- **Static optimisation:** Each worksheet represents a single-period decision problem and does not account for dynamic changes over time (e.g., seasonal variation or multi-period planning).

- **Operational simplification:** Real-world constraints such as labour availability, machine breakdowns, storage losses, and transport inefficiencies are not included.

- **Perfect efficiency assumption:** The model assumes full machine utilisation and no downtime, which may not reflect real operational conditions.


---

## Executive Decision Insights (Managerial Summary)

This Linear Programming model translates directly into actionable operational decisions for agricultural and agro-processing systems:

- **Cost optimisation in feed production:** The model identifies a least-cost feed formulation at ₦148.61/kg while still meeting all nutritional requirements, demonstrating how ingredient substitution can significantly reduce production costs.

- **Profit maximisation under capacity constraints:** Production scheduling shows that maximum profit (270) is achieved only when both machines are fully utilised, confirming that capacity—not demand—is the primary production bottleneck.

- **Optimal production balance:** The 60:60 maize-to-yam flour mix represents a structurally efficient production equilibrium, where both machine constraints are simultaneously binding.

- **Investment implications:** Since both Machine I and II operate at full capacity in the optimal solution, any increase in production requires capital investment in additional processing capacity rather than operational adjustments.

- **Decision transition impact:** The model demonstrates a shift from intuition-based decision-making to optimisation-driven planning, enabling more efficient allocation of scarce agricultural and processing resources.

---


## Summary

This project demonstrates how Linear Programming can:
- Minimise feed production costs
- Maximise agro-processing profits
- Optimise constrained machine allocation

It provides a **replicable optimisation framework for agricultural and food system decision-making**, particularly in resource-limited environments.























