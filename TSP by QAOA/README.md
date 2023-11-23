
Quantum Approximate Optimization Algorithm (QAOA) for TSP.

Overview:
This repository demonstrates the application of the Quantum Approximate Optimization Algorithm (QAOA) to solve the Traveling Salesman Problem (TSP). TSP involves finding the shortest possible route that visits a set of cities and returns to the starting city. Both classical and quantum solutions are presented for comparison.

Classical TSP Solution:
A classical brute-force algorithm is employed to explore all possible permutations of the cities, determining the order that minimizes the total distance traveled. The results are visualized on the TSP graph, showcasing the optimal route.

Quantum TSP Solution:
1. Conversion to Quadratic Program:
The TSP instance is converted into a Quadratic Program (QP), where the objective is to minimize the total distance traveled. Constraints ensure that each city is visited exactly once.

2. Mapping to Ising Hamiltonian:
The Quadratic Program is mapped to an Ising Hamiltonian, a form suitable for quantum computation. This mapping allows leveraging quantum algorithms for optimization.

3. Solving with Classical Eigensolver:
The Quadratic Program is solved using the exact classical eigensolver, establishing a baseline for comparison with quantum solutions.

4. Quantum Approximate Optimization Algorithm (QAOA):
QAOA is employed to find the optimal solution on a quantum computer. The algorithm uses a parameterized quantum circuit to evolve a quantum state, with parameters optimized to minimize the energy of the Ising Hamiltonian.

5. Results and Visualization:
Results from both classical and quantum solutions are presented, including the optimal route, objective function values, and computation times. Visualizations illustrate the optimal solutions on the TSP graph.
