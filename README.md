# QSP_Paper_Artifact
This Repo contains two jupyter notebook files that demonstrate two examples of the circuit proposed in https://arxiv.org/pdf/2303.02131.pdf (need to update to the latest arXiv version):

1. A 1+2 version (n = 3, m = 1) with all quantum gates hard-coded (O(logN depth with O(N) qubits). All gate sequences and oracles are implemented exactly as defined in the paper.
2. A 2+2 version (n = 4, m = 2) with all quantum gates hard-coded (O(logN depth with O(N) qubits). We do not implement the COPY oracles to save some qubit counts.

We also sorted some classical helper functions together into helper_function.py.

Please contact kgui@uchicago.edu if you have any questions.
