# FootLocker_discount_optimization

## Overview
This project attempts to address the current issue Foot-Locker has with selling shoes at a profit while being able to efficiently clean shelf space. Using a synthetic data set to simulate Foot-Lockers current business practices this notebook attempts to find optimal solutions.

## Business Problem
Currently one of the problems with Foot Locker is that it has a lot of shoes that are not selling and are taking up shelf space. In order to combat the waste of space, the company is considering slashing prices, trying to sell the excess stock at the cost of a massive loss of profits. Simply put, expensive shoes sit on a shelf taking up space, while heavily discounted shoes lose the company money but free up space.
 As of the 2nd quarter financial report, Foot Locker’s proforma comps has decreased by 3.9%, signalling a decline of the company's profitability and future possibilities. Dick Sporting Goods need to increase the profit of Foot Locker as quickly as possible as they are currently facing a potential lawsuit from their shareholders due to this purchase not leading to the growth that was anticipated. These reasons are why trying to maximize profit was chosen as the primary objective. The secondary objective was chosen as Dicks Sporting Goods inherited Foot Lockers stock and stores, requiring them to figure out how to merchandise and price Foot Lockers inventory. If this system were to work, Dicks sporting goods could not only avoid the lawsuit but would be able to raise its own value as a company, turning around the loss that this purchase has brought.     



## Status
🚧 Work in Progress - Part 1: Optimization Engine (Unit 11)

## Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

## Setup

## Part 1: Optimization Engine (Complete ✓)

### What It Does
This optimization engine analyzes 100 possible combinations of discounting luxury and regular
to identify the Pareto frontier of efficient solutions that balance Profit 
vs Shelf Space.

### Key Findings
- 37% of solutions are Pareto optimal
- 63 dominated solutions were identified and should be avoided
- === KEY STRATEGIC POINTS ON THE PARETO FRONTIER ===

1. BALANCED STRATEGY (Maximize combined objectives)
   Decision Variables: 0.0, 0.4
   norm_Profit: 0.8
   norm_Space: 0.8
   Total: 1.6

2. EQUITY STRATEGY (Most equal outcomes)
   Decision Variables: 0.0, 0.4
   norm_Profit: 0.8
   norm_Space: 0.8
   Gap: 0.0

3. OBJECTIVE 1 PRIORITY (Maximize first stakeholder)
   Decision Variables: 0.0, 0.2
   norm_Profit: 1.0
   norm_Space: 0.3

4. OBJECTIVE 2 PRIORITY (Maximize second stakeholder)
   Decision Variables: 0.3, 0.4667
   norm_Profit: 0.5
   norm_Space: 1.0

5. WEIGHTED STRATEGY (60% objective 1, 40% objective 2)
   Decision Variables: 0.0, 0.4
   norm_Profit: 0.8
   norm_Space: 0.8

### Running the Analysis
1. Ensure you have the required packages: `pandas`, `numpy`, `matplotlib`
2. Open `optimization_engine.ipynb`
3. Run all cells in order
4. Outputs will be saved to the `images/` folder

### Next Steps
Part 2 will add a constraint-aware decision agent that selects among these
Pareto optimal solutions based on business constraints and priorities.

