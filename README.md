# Empirical Validation of Ancilla Recycling via Uncomputation and Loschmidt Echo Decay on NISQ Architectures

This repository contains the code, circuit descriptions, and raw measurement counts from experiments executed on IBM Quantum's 156-qubit superconducting hardware (`ibm_kingston`).

## Overview
- **Paper DOI:** [10.5281/zenodo.23696412](https://doi.org/10.5281/zenodo.23696412)
- **Hardware:** IBM Quantum `ibm_kingston` (156-qubit heavy-hex lattice)
- **Execution Date:** October 27, 2026
- **Framework:** Qiskit & Qiskit IBM Runtime

## Experimental Results Summary

| Experiment | Qubits | Register Measured | Job ID | Shots | Success Rate |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 12-Qubit Ancilla Reset | 12 | 6 Ancillas | `dbgc22djm0ks73egaq2g` | 1000 | 95.60% |
| 20-Qubit Uniform Uncomputation | 20 | 10 Ancillas | `dbgc310iudkc73e46hhg` | 1000 | 90.10% |
| 20-Qubit Parameterized Uncomputation | 20 | 10 Ancillas | `dbgc390iudkc73e46i70` | 1000 | 90.30% |
| 20-Qubit Full Loschmidt Echo | 20 | All 20 Qubits | `dbgc4i1j4t8s73ac2bcg` | 1000 | 21.40% |

## Repository Structure
- `notebooks/ancilla_uncomputation_benchmark.ipynb`: Full reproducible workflow.
- `data/`: Raw measurement count dictionaries (JSON) for each executed job.

## Citation
```bibtex
@article{mohan2026ancilla,
  title={Empirical Validation of Ancilla Recycling via Uncomputation and Loschmidt Echo Decay on NISQ Architectures},
  author={Mohan, Agaram Madhan},
  year={2026},
  doi={10.5281/zenodo.23696412}
}
