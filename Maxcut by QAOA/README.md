Quantum Approximate Optimization Algorithm (QAOA) for Maxcut.

Overview:
This repository focuses on solving the Maxcut problem using the Quantum Approximate Optimization Algorithm (QAOA). The Maxcut problem involves partitioning the nodes of a graph into two sets to maximize the sum of weights on the cut edges. The classical solution is presented alongside the quantum approach for comparison.

Classical Maxcut Solution:
A classical brute-force algorithm explores all possible binary configurations of the graph's nodes and identifies the one that maximizes the cut. The results are visualized on the graph, showcasing the optimal cut configuration.

Quantum Maxcut Solution:
1. Conversion to Quadratic Program:
The weight matrix of the graph is converted into a Quadratic Program (QP). The QP is formulated to maximize the sum of weights on the cut edges, representing the objective function of the Maxcut problem.

2. Mapping to Ising Hamiltonian:
The Quadratic Program is then mapped to an Ising Hamiltonian, a mathematical representation suitable for quantum computations. This transformation is essential for quantum optimization algorithms.

3. Solving with Classical Eigensolver:
The Quadratic Program is solved using the exact classical eigensolver, providing a baseline for comparison with quantum solutions.

4. Quantum Approximate Optimization Algorithm (QAOA):
The Quantum Approximate Optimization Algorithm (QAOA) is employed to find the optimal solution on a quantum computer. The algorithm uses a parameterized quantum circuit to evolve a quantum state, and the parameters are optimized to minimize the energy of the Ising Hamiltonian.

5. Results and Visualization:
Results from both classical and quantum solutions are presented, including the optimal cut configuration, objective function values, and computation times. Visualizations demonstrate the optimal solutions on the graph.
