# Hello Quantum world
Here, I use Qskit to demostrate how to write the quantum circuit. Initially, all qubits will be set up 0 state. After adding  Hadamard gate, we can get the qubit zero with the superposition 0 and 1. By applying CNOT gate on qubit 1 (targaet qubit) and qubit 0 (control qubit), we can get Bell state.

# Bit flip code
The bit flip code is a simple code to demostrate how the quantum algorithm to correct the errors generated from the noise. Here, we also design a error simulator which flips the qubit with probability p. In Qskit, quantum gates, qubits, and measurement are prefect. However, in real quantum computer, the physical qubit will decohere due the noise. The logical gate cannot operate the qubit well. Lots of reason induce the errors in the quantum computation. Therefore, for the quantum algorithm, one can design the code to correct the error from noise. The bit flip code is one of quantum error correction code and the most simple one. 

