# Predictive Machine Maintenance Using Markov Process

## Overview
This project uses a **Markov Chain Model** to simulate machine health conditions and predict possible transitions toward machine failure. It demonstrates how Markov Processes can support preventive maintenance planning in manufacturing industries.

## Objective
To predict machine health states and failure probability using a Markov Process, helping plan preventive maintenance and reduce machine downtime.

## Problem Statement
Machines in manufacturing industries gradually degrade over time. If maintenance is not performed at the right time, machines may fail and interrupt production. This project models machine health transitions using a Markov Chain.

## Machine States

| State | Description |
|---|---|
| S1 | Fully Operational |
| S2 | Minor Wear |
| S3 | Major Fault |
| S4 | Machine Failure |

## Transition Probability Matrix

| Current State | S1 | S2 | S3 | S4 |
|---|---:|---:|---:|---:|
| S1 | 0.7 | 0.2 | 0.1 | 0.0 |
| S2 | 0.2 | 0.5 | 0.2 | 0.1 |
| S3 | 0.0 | 0.3 | 0.4 | 0.3 |
| S4 | 0.0 | 0.0 | 0.0 | 1.0 |

The matrix defines the probability of a machine moving from its current health state to another state.

## Technologies Used
- Python
- NumPy
- Matplotlib
- Jupyter Notebook

## Implementation
1. Define machine health states.
2. Create the transition probability matrix.
3. Simulate machine behavior using random state transitions.
4. Record machine states over time.
5. Visualize state transitions using a graph.

## How to Run
1. Install Python or Anaconda.
2. Install the required libraries:

   ```bash
   pip install numpy matplotlib notebook
   ```

3. Open the notebook in Jupyter Notebook.
4. Run all cells in order.

## Expected Output
- Simulated machine states printed in the notebook.
- A graph showing machine-state transitions over time.

**Note:** Results may vary between runs because the simulation uses random transitions. The probabilities are example values, not predictions trained on real machine sensor data.

## Applications
- Machine health monitoring
- Machine degradation modelling
- Failure-state simulation
- Preventive maintenance planning

## Conclusion
This project demonstrates how a Markov Process can model machine health transitions using probabilities. It provides a basic simulation that can help explain machine degradation and support maintenance planning.
