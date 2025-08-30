# Linear Programming Applications in Agricultural and Food Production

*This project demonstrates practical applications of Linear Programming (LP) in optimizing agricultural and food production decisions, including nutrient-cost optimization, production scheduling, and machine allocation for small-scale processing plants.*

[![📊 Linear Programming Optimization ⚙️](https://img.shields.io/badge/GitHub-📊_Linear_Programming_⚙️-green?logo=github&labelColor=darkgreen)](https://github.com/Lauren-Akhidenor/LINEAR-PROGRAMMING/edit/main/README.md)

---

## 📑 Table of Contents
1. [Project Overview](#-project-overview)
2. [Problem Worksheets](#-problem-worksheets)
   - [Worksheet 1: Nutrient-Cost Optimization](#worksheet-1-nutrient-cost-optimization)
   - [Worksheet 2: Production Scheduling](#worksheet-2-production-scheduling)
   - [Worksheet 3: Machine Allocation](#worksheet-3-machine-allocation)
3. [Methods](#-methods)
4. [Results & Metrics](#-results--metrics)
5. [Insights](#-insights)
6. [How to Run](#-how-to-run)
7. [Contributing](#-contributing)

---

## Project Overview
Linear Programming is a mathematical method for determining the best possible outcome (such as maximum profit or minimum cost) in a given model with **constraints**. This project explores three LP scenarios:

1. **Nutrient-Cost Optimization:** Determine the optimal mix of grains to meet nutrient requirements at minimum cost.  
2. **Production Scheduling:** Allocate machine time to maximize profit from Maize Flour and Yam Flour production.  
3. **Machine Allocation:** Evaluate feasible allocations for machine usage to meet production targets while adhering to capacity constraints.

Data is provided in spreadsheets, and solutions are obtained using **Excel Solver / LP optimization tools**.

---

## Worksheets

### Worksheet 1: Nutrient-Cost Optimization
| Nutrient / Cost | Grain 1 | Grain 2 | Grain 3 | Minimum Requirement | Minimum Achieved |
|-----------------|--------|--------|--------|------------------|----------------|
| Nutrient A      | 20     | 30     | 70     | 110              | 110            |
| Nutrient B      | 10     | 10     | 0      | 18               | 26.03          |
| Nutrient C      | 50     | 30     | 0      | 90               | 90             |
| Nutrient D      | 6      | 2.5    | 10     | 14               | 14             |
| Cost (₦/Kg)    | 41     | 36     | 96     |                  | 148.61         |

- **Decision Variables:** Quantity of each grain to meet nutrient requirements.  
- **Objective Function:** Minimize total cost.  
- **Constraints:** Minimum nutrient requirements per nutrient type.  

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

- **Objective Function:** Maximize profit.  
- **Constraints:** Machine time limitations (Machine I and II).  

---

### Worksheet 3: Machine Allocation for Maize and Yam Flour
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

- **Purpose:** Evaluate feasible allocations and identify the optimal production mix under machine constraints.  

---

## Methods
- **LP Modeling:** Formulate objective functions, constraints, and decision variables for each problem.  
- **Solver / Optimization:** Excel Solver was used for all three worksheets to find the **optimal solution**.  
- **Validation:** Ensure constraints are satisfied while maximizing/minimizing objectives.

**Formulas used for LP:**
- Total Cost = Σ (Cost per unit × Quantity of each grain)  
- Total Profit = Σ (Profit per unit × Quantity produced)  
- Constraints: Σ (Nutrient contribution × Quantity) ≥ Minimum Requirement  
- Machine time: Σ (Machine usage per product × Quantity) ≤ Machine availability  

---

## Results & Metrics

- **Worksheet 1:** Optimal grain mix meets all nutrient requirements at a **minimum total cost of ₦148.61/kg**.  
- **Worksheet 2:** Optimal production scheduling maximizes profit while using available machine time efficiently.  
- **Worksheet 3:** Feasible machine allocations determined for different production levels to maintain operational efficiency.  

---

## Insights
- LP enables **cost-efficient nutrition planning** using multiple grain types.  
- Production scheduling can **maximize profit** under resource constraints.  
- Machine allocation analysis ensures **optimal usage of limited processing capacity**.  
- These methods can be applied in **agriculture, food processing, and small-scale industry planning**.

---


## Graphics & Visualizations

### Worksheet 1: Nutrient-Cost Optimization
<details>
<summary>Click to expand Nutrient-Cost Charts</summary>

<img src="Screenshot (961).png" width="700">
<img src="Screenshot (962).png" width="700">

</details>

### Worksheet 3: Machine Allocation
<details>
<summary>Click to expand Machine Allocation Charts</summary>

<img src="Screenshot (964).png" width="700">

</details>


---

## 🚀 How to Run
```bash
git clone https://github.com/Lauren-Akhidenor/LP-Projects.git
cd LP-Projects
# Open the Excel sheets and use Solver to replicate results
