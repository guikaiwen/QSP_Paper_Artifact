# QSP_Paper_Artifact
This Repo contains two Jupyter Notebook files that demonstrate two examples of the low-depth quantum state preparation (QSP) protocol proposed in https://arxiv.org/pdf/2303.02131.pdf, using the Braket SDK:

1. `1+2_Circuit_With_COPY_Braket.ipynb`: A 1+2 version ($n = 3$, $m = 1$) with all quantum gates hard-coded. All gate sequences and operations are implemented exactly as defined in the paper.
2. `2+2_Circuit_Braket.ipynb`: A 2+2 version ($n = 4$, $m = 2$) with all quantum gates hard-coded. We do not implement the COPY operations to save some ancilla qubits.

(Note that $N = 2^n$ is the total number of amplitude values encoded, and $n$ can also represent the number of data qubits.)

We also sorted some classical helper functions together into `helper_function.py`.

-------------------------------

The Amazon Braket Python SDK can be installed with pip on your local machine as follows:
```ruby
pip install amazon-braket-sdk
```
See https://pypi.org/project/amazon-braket-sdk/ for more installation details.

The current Braket SDK version is `1.55.0`.

-------------------------------
The current QSP operation demonstrated in this repo has the following circuit complexity numbers:

A. $O(\log(N))$ depth using arbitrary single qubit gate + CNOT gate

B. $O(N)$ ancilla qubits required

(Note that $N = 2^n$ is the total number of amplitude values encoded, and $n$ can also represent the number of data qubits.)

-------------------------------
Please contact kgui@uchicago.edu if you have any questions.
