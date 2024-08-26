# ProductionPlanningUsing_GRASP

**Problem Definition**
The goal is to assign orders to a set of production lines at the company's sites to maximize revenue. Each order has an associated production time and revenue. Additionally, cost savings can be achieved when specific products are produced on the same production line.

This script outlines the implementation of a Greedy Randomized Adaptive Search Procedure (GRASP) for solving the Planning problem. To be more precise the framework that is being used is the Reactive GRASP. The algorithm aims to maximize the revenue while considering the cost savings from pairing orders on the same production line.

### Key aspects of this algorithm include:
-   **Neighborhood Operator**: Utilizes swap moves between order lines to explore the solution space.
-   **Termination Criteria**: The algorithm terminates based on a predefined time limit, ensuring timely execution.
-   **Step Criterion**: Employs the "Best Improvement" strategy for selecting the next move, focusing on the most beneficial swap.
-   **Cost**: Operates with a revenue matrix for individual orders and a cost-saving matrix for order pairs, derived from an input file.
-   **Initialization**: Implements a Greedy Randomized Cnstruction heuristic for generating an initial solution.
-   **Reactive GRASP**: Adjusts the greediness level (α) dynamically, balancing exploitation and exploration to improve solution quality over iterations.

