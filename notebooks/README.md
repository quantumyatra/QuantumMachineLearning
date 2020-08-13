# Updates in the notes 

Because of updates in the qiskit some of the functions/classes are deprecated. Here is the list of fixes for the notes

* 01_Classical_and_Quantum_Probability_Distributions
    * Replace `circuit.iden(q[0])` by `circuit.i(q[0])` as circuit.iden is deprecated
* 05_Gate-Model_Quantum_Computing
    * Replace `compiled_circuit.as_dict()['experiments'][0]['instructions']`  by `compiled_circuit.experiments[0].instructions` As the `assemble` returns an object and `experiments` is one of the functions.
* 07_Variational_Circuits.ipynb 
    * Completely remove `from qiskit.aqua import get_aer_backend`, and instead use `Aer.backends(name_of_your_simulator)`
