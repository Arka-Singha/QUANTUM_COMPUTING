# Grover's Algorithm Simulation using Qiskit

A Python-based simulation and visualization of **Grover’s Search Algorithm** using IBM's Qiskit framework. This project demonstrates how quantum computing can speed up unstructured search problems that are classically time-consuming.

---

## 🧠 What is Grover's Algorithm?

Grover’s Algorithm is a **quantum algorithm for searching an unsorted database** or solving the "black-box" function problem. It provides a **quadratic speedup** over classical brute-force search.

- **Classical search:** O(N) time to find an item in an unsorted list of N elements.
- **Grover’s quantum search:** O(√N) time complexity.

It works by:
1. Initializing a quantum superposition of all states.
2. Applying an **oracle** that marks the correct state.
3. Amplifying the probability of the correct state using **Grover's Diffusion Operator**.
4. Measuring the quantum state to extract the answer.

---

## 📁 Project Structure

This Jupyter Notebook contains:

- ✅ Initialization of a 2-qubit/3-qubit quantum system
- 🧿 Oracle design for marking the solution
- 🔄 Implementation of the Grover iteration (oracle + diffusion)
- 📈 Visualization of state probabilities using Qiskit
- 🧪 Simulation of final state measurement
- 📚 Optional theoretical explanation and math

---

## 🛠️ Requirements

- Python 3.7+
- [Qiskit](https://qiskit.org/)
- Jupyter Notebook or VS Code with Jupyter support
- Matplotlib (for visualization)

## Quantum Circuits
![image](https://github.com/user-attachments/assets/e12134e9-4751-4862-994a-ac7d1a955884)

![image](https://github.com/user-attachments/assets/b5983f1f-39c7-442d-95dc-18ca5b99ccc7)

![image](https://github.com/user-attachments/assets/d97a0070-0632-4816-b5d6-f7d48db4a812)

![image](https://github.com/user-attachments/assets/6fd19b17-d6fe-47ff-873b-52c02b918d06)


## RESULTS: 
![image](https://github.com/user-attachments/assets/163e452d-25ce-45cb-9d05-3bb3bcb7e854)
![image](https://github.com/user-attachments/assets/e71d5581-ca78-41e7-8774-20ecbde1e077)
![image](https://github.com/user-attachments/assets/887ecac8-b477-4b36-aba7-2f52af24592a)

The implementation of Grover’s Algorithm in this project demonstrates a 3-qubit quantum circuit that efficiently locates a marked state using quantum amplitude amplification. The oracle circuit identifies the target state by flipping its phase, while the diffusion operator enhances its probability through inversion about the mean. The full pipeline includes superposition initialization, oracle application, diffusion, and measurement. Simulation results show that the algorithm successfully amplifies the correct state (e.g., `|100⟩`) with high probability (~0.5), as visualized in the bar plots. The consistency across multiple runs confirms the accuracy and repeatability of the algorithm, highlighting Grover’s quadratic speedup for unstructured search problems.
  

## 💡Applications
Grover’s algorithm can be extended to solve:
* Cryptographic key search (e.g., symmetric key attacks)
* Sudoku puzzles and combinatorial optimization
* Database lookups and pattern matching
* NP-complete decision problems (with caveats)

## 📚 References

* Michael A. Nielsen and Isaac L. Chuang, _Quantum Computation and Quantum Information_
* Qiskit Textbook: Grover's Algorithm
* MIT OCW: Quantum Algorithms
