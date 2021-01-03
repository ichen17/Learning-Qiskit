# Hello Quantum world
Here, I use Qiskit to demostrate how to write the quantum circuit. Initially, all qubits will be set up 0 state. After adding  Hadamard gate, we can get the qubit zero with the superposition 0 and 1. By applying CNOT gate on qubit 1 (targaet qubit) and qubit 0 (control qubit), we can get a Bell state.

# Bit flip code
The bit flip code is a simple code to demostrate how the quantum algorithm to correct the errors generated from the noise. Here, we also design a error simulator which flips the qubit with the probability p. In Qiskit, quantum gates, qubits, and measurements are ideal (not influenced by noises). However, in real quantum computer, the physical qubit will decohere due to the noise. The logical gate cannot operate the qubit well. There are lots of factors inducing the errors in the quantum computation. Therefore, for the quantum algorithm, one can design the code to correct the error from noise. The bit flip code is one of quantum error correction code and the most simple one. 

Here, we use two ancilla qubits to encode the information from a physical qubit. For example, |0> will be encode into |000>. Each of them have the chance p to flip the bit 0 -> 1. The state will become |001>, |100>..... After the ocurrence of bit flipping, one can decode the information. Decoding the information is just like counting the bit and use dominated one as the  correct information. For instance,  |100> will be decoded as |011> and |011> -> |111>. The first bit represents the physical bit we want to correct. With this error correction code, the probability of measure a correct physical qubit is (1-P)^3 + 3p(1-P)^2. If p > 0.5, the probability of error occurrence is lower than one without the error correction.  

# Superdense Code
The superdense Code is similiar to the quantum teleportation. However, the difference between them is the information they send. For the superdense code, the code is used to transport the classical information like '00', '01'. On the other hand, the quantum teleportation is used to transport quantum information like superposition of '01' and '00'. 

In Qiskit textbook, they said the third party will prepare the Bell pair and send one of them to Alice and another of them to Bob. Alice make the operation on her own qubit and send it to Bob. Therefore, by just disentangling the Bell pair,Bob will know the information that Alice send.    

# Deutsch-Jozsa Algorithm
Deutsch-Jozsa Algorithm is the first quantum algorithm that demostrate Quantum algorithm faster than the best classical algorithm. Deutsch-Jozsa problem to identify whether f(x) is a balenced function or a constant function. 

# Bernstein-Vazirani Algorithm

