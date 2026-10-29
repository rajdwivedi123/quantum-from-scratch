# quantum-from-scratch
Building a Quantum Simulator from Scratch
Quantum Computing from Scratch
Learning quantum computing by building it myself, starting from plain NumPy and working up to running circuits on real quantum hardware.
The idea is simple: before using a quantum library like Qiskit, write the core pieces by hand. Qubit states are complex vectors, gates are matrices, and measurement probabilities are squared magnitudes. Building those from scratch makes it clear what the libraries are actually doing.
Roadmap
[x] Phase 1a: NumPy foundations. Arrays, indexing, slicing, broadcasting, boolean masks, dtypes, and NumPy's numerical edge cases (NaN, overflow, floating-point precision)
[ ] Phase 1b: Complex linear algebra. Complex vectors, conjugates, normalization, the Kronecker product, unitary matrices
[ ] Phase 2: Quantum simulator in NumPy. Single-qubit states and gates, measurement, multi-qubit systems, CNOT, Bell states
[ ] Phase 3: Qiskit. Rebuild the simulator's circuits in Qiskit and check that the results match
[ ] Phase 4: Algorithms and hardware. Grover's search, the quantum Fourier transform, and running circuits on real IBM quantum hardware
Notebooks
Notebook	Contents	Status
`01_numpy_exercises.ipynb`	Exercises 1–51 of the 100 NumPy exercises	Done
`02_complex_linear_algebra.ipynb`	Complex vectors, normalization, `np.kron`, gate matrices	In progress
`03_quantum_simulator.ipynb`	A state-vector quantum simulator written in NumPy	Planned
Each notebook can be opened and run in Google Colab with no installation.
Highlights so far
Built and normalized a first qubit state, `[0.5+0.5j, 0.5-0.5j]`, an equal superposition of 0 and 1
Worked through why `0.3 == 3 * 0.1` is `False`, and why comparing floats needs a tolerance (`np.allclose`)
Saw how NaN silently turns into a huge negative number when converted to an integer
Learned why the Kronecker product makes a quantum state's size grow as 2ⁿ, and why that makes quantum systems so hard to simulate classically
Resources
100 NumPy exercises
IBM Quantum Learning
PennyLane Codebook
