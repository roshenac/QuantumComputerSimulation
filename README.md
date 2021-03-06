# Simulation of a Quantum Computer

## Description
A simulation of a quantum computer was implemented on a classical computer using the Java programming language. All basic components of a quantum computer were created and the Deutsch-Jozsa algorithm, Grover’s quantum search algorithm and Shor’s integer factorisation algorithm were implemented and successfully run. Shor’s algorithm was used to factor 15 and 21 into their primes using a personal computer.

## Design 
The design of the implemented quantum computer simulation is based on a library design pattern. As such there is no strict usage of the source code, a host program simply imports the packages it requires. The source code was packaged into discrete packages to enable maximum extendibility. Four main packages are contained in the project: Core, Core.Math, Operators and Algorithms. The Core package contains the fundamental classes required to represent a quantum computer, with the Core.Math package containing the mathematical structures required. The Operators and Algorithms packages are extensions of the Core package, which implement common operators and algorithms on quantum computers.
The Core package contains a single implementation: QRegister, representing a quantum register and three interfaces, Operator, Algorithm, AlgorithmOutput. The Operator interface is a representation of a linear operator and its interaction with QRegister objects. The Algorithm interface is defined such that an Algorithm has a run method, either classical or quantum. In combination with Algorithm we needed a variable output type to be the result of all algorithms, the AlgorithmOutput interface represents this in such a way that the only requirement of the output of an algorithm is that it has a human readable string associated with it.

## Authors
* Roshenac Mitchell
* Max Nolte
* Martin Ru ̈fenacht
* Mark Stringer
* Justs Zarin ̧ ̆s
