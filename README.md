Task 1 

The Swap test is a simple quantum circuit which, given two states, allows to compute how much do they differ from each other.

Provide a variational (also called parametric) circuit which is able to generate the most general 1 qubit state. By most general 1 qubit state we mean that there exists a set of the parameters in the circuit such that any point in the Bloch sphere can be reached. Check that the circuit works correctly by showing that by varying randomly the parameters of your circuit you can reproduce correctly the Bloch sphere.
Use the circuit built in step 1) and, using the SWAP test, find the best choice of your parameters to reproduce a randomly generated quantum state made with 1 qubit.
Suppose you are given with a random state, made by N qubits, for which you only know that it is a product state and each of the qubits are in the state | 0 > or | 1>. By product state we mean that it can be written as the product of single qubit states, without the need to do any summation. For example, the state
|a> = |01>
Is a product state, while the state
|b> = |00> + |11>
Is not.

Perform a qubit by qubit SWAP test to reconstruct the state. This part of the problem can be solved via a simple grid search.


Task 3
Learning by doing: the best way to understand the basics of quantum computation is to implement a quantum circuit simulator. This task is suitable both for people from computer sciences who want to learn about quantum computing, and for people from math/physics who want to exercise coding.

Detailed description of the task with some learning resources and examples can be found in this jupyter notebook

It is expected that simulator can perform following:
initialize state
read program, and for each gate:
calculate matrix operator
apply operator (modify state)
perform multi-shot measurement of all qubits using weighted random technique


Task 4 
The MaxCut problem is a well-known optimization problem in which the nodes of a given undirected graph have to be divided in two sets (often referred as the set of “white” and “black” nodes) such that the number of edges connecting a white node with a black node are maximized. The MaxCut problem is a problem on which the QAOA algorithm has proved to be useful (for an explanation of the QAOA algorithm you can read this blogpost).

At this link you can find an explicit implementation of the QAOA algorithm to solve the MaxCut problem for the simpler case of an unweighted graph. We ask you to generalize the above code to include also the solution for the case of weighted graphs.
