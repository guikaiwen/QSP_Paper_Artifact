# QSP_Paper_Artifact
This Repo contains two jupyter notebook files that demonstrate two examples of the circuit proposed in https://arxiv.org/pdf/2303.02131.pdf:

1. `1+2_Circuit_With_COPY_Braket.ipynb`: A 1+2 version (n = 3, m = 1) with all quantum gates hard-coded. All gate sequences and oracles are implemented exactly as defined in the paper.
2. `2+2_Circuit_Braket.ipynb`: A 2+2 version (n = 4, m = 2) with all quantum gates hard-coded. We do not implement the COPY oracles to save some qubit counts.

(Note that $N = 2^n$ is the total number of amplitude values encoded, and $n$ can also represent the number of data qubits.)

We also sorted some classical helper functions together into `helper_function.py`.

-------------------------------
The current QSP operation demonstrated in this repo has the following circuit complexity numbers:

A. $O(\log(N))$ depth using arbitrary single qubit gate + CNOT gate

B. $O(N)$ ancilla qubits required

(Note that $N = 2^n$ is the total number of amplitude values encoded, and $n$ can also represent the number of data qubits.)

See https://github.com/guikaiwen/qubit_efficient_QSP for an alternative method that has the following circuit complexity numbers:

A. $O(N)$ depth using generalized multi-controlled Ry gates

B. No additional ancilla qubits required (total of $O(\log(N))$ qubits)

-------------------------------
Please contact kgui@uchicago.edu if you have any questions.
