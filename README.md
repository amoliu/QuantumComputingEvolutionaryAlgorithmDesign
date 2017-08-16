## QuantumComputingEvolutionaryAlgorithmDesign

# Description
Uses evolutionary algorithms and python-quintuple to automatically design quantum computing algorithms. Inspired by the ideas in the following PhD thesis, but implemented entirely originally, http://theses.ucalgary.ca/jspui/bitstream/11023/2780/3/ucalgary_2016_zahedinejad_ehsan.pdf,.

# Operation.
The algorithm maps the complete set of quantum gates T, Hadamard, CNOT, and their relative positions as a simple 'DNA', a generation of multiple random quantum algorithm 'DNA' are generated and compared to the desired output quantum state, the best members of this generation are bred (cut and joined together) and mutated (random 'DNA' changes) to create the next generation which is again evaluated.

Example of a 5-qbit algorithm 'DNA'
    |    T    . - (+)    |
    |    |    |    H    T
    |    T    |    |    T
    H    |    |    H    |
    . - (+)    T    T    H
    . - (+)    T    T    |
    |    |    T    . - (+)
    |    |    T    T    |
    . - (+)    |    . - (+)

# Inputs and Targets
The required inputs and outputs for an algorithm are supplied as a series of probabilities, for instance a 2 qbit inversion gate could have the following inputs [[0, 0], [0, 1], [1, 0], [1, 1]] and following outputs [[1, 1], [1, 0], [0, 1], [0, 0]].

# To Do.
Implement more algorithm examples and working case studies.
