# Linear Programming Applications in Agricultural and Food Production

*This project demonstrates the use of Linear Programming (LP) to optimise agricultural and food production decisions, including nutrient-cost optimisation, production scheduling, and machine allocation for small-scale processing, with implications for efficiency, profitability, and sustainable resource management.*

[![📊 Linear Programming Optimisation ⚙️](https://img.shields.io/badge/GitHub-📊_Linear_Programming_⚙️-F5F5DC?logo=github&logoColor=white&labelColor=800020)](https://github.com/Lauren-Akhidenor/LINEAR-PROGRAMMING/edit/main/README.md)

---

## 📑 Table of Contents
1. [Project Overview](#project-overview)
2. [Economic & Analytical Methodology](#economic--analytical-methodology)
3. [Problem Worksheets](#problem-worksheets)
   - [Worksheet 1: Nutrient-Cost Optimisation](#worksheet-1-nutrient-cost-optimisation)
   - [Worksheet 2: Production Scheduling](#worksheet-2-production-scheduling)
   - [Worksheet 3: Machine Allocation](#worksheet-3-machine-allocation)
4. [Results & Metrics](#results--metrics)
5. [Critical Practical Applications](Critical-Practical-Applications)
6. [Insights & Implications](#insights--implications)
7. [Summary](Summary)


---

## Project Overview
Linear Programming is a mathematical optimisation tool used to determine the **best possible outcome** under a set of constraints, such as maximising profit or minimising cost. This project explores three LP applications in agricultural and food production:

1. **Nutrient-Cost Optimisation:** Identify the cost-minimising combination of grains to meet daily nutrient requirements.  
2. **Production Scheduling:** Allocate machine time to maximise profit from Maize Flour and Yam Flour production.  
3. **Machine Allocation:** Optimise machine usage to meet production targets whilst respecting capacity constraints.  

The solutions provide **evidence-based insights** for farm-level decision-making and small-scale food processing efficiency.

---

## Economic & Analytical Methodology
This project applies **quantitative optimisation and economic evaluation principles** to agricultural production:

- **Linear Programming (LP):** Formulate objective functions (cost or profit) and constraints (nutrient requirements, machine capacity, production limits).  
- **Decision Variables:** Quantities of grains or units of products to produce.  
- **Solver Optimisation:** Excel Solver identifies the optimal solution that satisfies all constraints.  
- **Economic Metrics:** Total cost, total profit, and efficiency ratios are analysed to support **resource allocation and policy decisions**.  
- **Validation:** Ensure all constraints are satisfied whilst achieving maximum economic efficiency.

This approach enables **data-driven recommendations** for cost reduction, productivity enhancement, and sustainable resource use in agricultural systems.

---

## Problem Worksheets

### Worksheet 1: Nutrient-Cost Optimisation
| Nutrient / Cost | Grain 1 | Grain 2 | Grain 3 | Minimum Requirement | Minimum Achieved |
|-----------------|--------|--------|--------|------------------|----------------|
| Nutrient A      | 20     | 30     | 70     | 110              | 110            |
| Nutrient B      | 10     | 10     | 0      | 18               | 26.03          |
| Nutrient C      | 50     | 30     | 0      | 90               | 90             |
| Nutrient D      | 6      | 2.5    | 10     | 14               | 14             |
| Cost (₦/Kg)    | 41     | 36     | 96     |                  | 148.61         |

- **Decision Variables:** Quantities of each grain.  
- **Objective Function:** Minimise total cost whilst meeting nutrient requirements.  
- **Constraints:** Minimum required nutrient levels per nutrient type.  

---

### Worksheet 2: Production Scheduling
| Product      | Maize Flour | Yam Flour | Notes           |
|-------------|------------|-----------|----------------|
| Decision Variable | 60         | 60        | Initial guess |
| Machine I (min/unit) | 3          | 2         | Minutes per unit |
| Machine II (min/unit) | 2          | 4         | Minutes per unit |
| Total Machine I       | 300        |           | Total used |
| Total Machine II      | 360        |           | Total used |
| Available Machine I   | 300        |           | Maximum capacity |
| Available Machine II  | 360        |           | Maximum capacity |
| Total Profit          | 270        |           | Profit formula |

- **Objective Function:** Maximise profit.  
- **Constraints:** Machine capacity and production requirements.  

---

### Worksheet 3: Machine Allocation
| Maize Flour (x_M) | Yam Flour (Machine I) | Yam Flour (Machine II) |
|------------------|---------------------|----------------------|
| 0                | 150                 | 90                   |
| 10               | 135                 | 85                   |
| 20               | 120                 | 80                   |
| 30               | 105                 | 75                   |
| 40               | 90                  | 70                   |
| 50               | 75                  | 65                   |
| 60               | 60                  | 60                   |
| 70               | 45                  | 55                   |
| 80               | 30                  | 50                   |
| 90               | 15                  | 45                   |
| 100              | 0                   | 40                   |

- **Purpose:** Identify optimal production mix whilst meeting machine constraints.  

----

## Graphics & Visualisations

### Worksheet 1: Nutrient-Cost Optimisation
<details>
<summary>Click to expand Nutrient-Cost Charts</summary>
<img src="Screenshot (961).png" width="700">
</details>

### Worksheet 2: Maximised Profit
<details>
<summary>Click to expand Nutrient-Cost Charts</summary>
<img src="Screenshot (962).png" width="700">
</details>

### Worksheet 3: Machine Allocation
<details>
<summary>Click to expand Machine Allocation Charts</summary>
<img src="Screenshot (964).png" width="700">
</details>

---

## Results & Metrics
- **Worksheet 1:** Achieved minimum total cost (₦148.61/kg) whilst meeting all nutrient requirements.  
- **Worksheet 2:** Maximised profit under available machine time.  
- **Worksheet 3:** Determined feasible allocations to optimise production efficiency.  
- **Analytical Impact:** Quantified trade-offs between cost minimisation and production capacity, informing resource allocation decisions.

---


## Critical Practical Applications

### For Feed Millers & Livestock Farmers
- LP eliminates guesswork in ration formulation  
- **Nutrient B achieved 26.03 vs 18 minimum** (44% surplus), opportunity to reduce feed costs further  
- Re-optimize formulations whenever grain prices change  

### For Small-Scale Processors
- Both machines operating at 100% capacity are **binding constraints**  
- **Investment priority:** expand Machine I or II based on sensitivity analysis  
- **60:60 Maize:Yam ratio** maximizes current equipment efficiency  

### For Extension & Training
- **Excel Solver is free and accessible**, offering a low barrier to adoption  
- **Visual trade-off curves (Worksheet 3)** help farmers intuitively understand optimization  
- Templates can be localised for different crops or products  

---

## Insights & Implications
- LP provides **cost-efficient, data-driven decision-making** for nutrition planning and production scheduling.  
- Resource allocation analysis ensures **optimal use of limited farm and processing inputs**.  
- Methods can guide **policy recommendations** for smallholder farming efficiency and sustainable agri-business planning.  
- Demonstrates how **quantitative modelling and economic evaluation** can drive actionable insights in agricultural systems.


---

**Summary:**  
LP optimization provides actionable guidance for **cost-efficient feed formulation, profit-maximizing production schedules, and effective machine allocation**. These insights support smallholders, processors, and extension services to make data-driven operational decisions.


----

---

