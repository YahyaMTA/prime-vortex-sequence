# Prime Vortex Sequence

This repository contains SageMath code and supporting materials for the paper:

"The Prime Vortex Sequence"
John V. Teixido, 2025
Submitted to SIAM Journal on Applied Dynamical Systems

Overview

This project implements the Prime Vortex Sequence, a new class of integer sequences defined by alternating prime-based growth and composite-based reduction. 

The code enables:

    Generation of the sequence for arbitrary starting values and parameter $a$

    Detection and analysis of cycles

    Reproduction of all computational results and tables from the associated paper

Mathematical Definition

The Prime Vortex Sequence is defined recursively as follows:
nk+1={ank+nextprime(nk),if nk is primenkspf(nk),if nk is composite
nk+1=⎩
⎨
⎧ank+nextprime(nk),spf(nk)nk,if nk is primeif nk is composite

where:

    $\mathrm{nextprime}(n_k)$ is the smallest prime greater than $n_k$

    $\mathrm{spf}(n_k)$ is the smallest prime factor of $n_k$

For example, starting with $n_0 = 7$ and $a = 2$:

    $n_1 = 2 \cdot 7 + 11 = 25$

    $n_2 = 25 / 5 = 5$

    $n_3 = 2 \cdot 5 + 7 = 17$

    $\ldots$

How to Run
Requirements

    SageMath (version 9.0 or later recommended)

    Python 3.x (if running standalone Python scripts)

Instructions

    Clone the repository:

bash
git clone https://github.com/your-username/prime-vortex-sequence.git
cd prime-vortex-sequence

Open the main SageMath file:

    prime_vortex_sequence.ipynb

Run in SageMath:

    From the command line:

        bash
        sage prime_vortex_sequence.sage

        Or open the notebook in SageMath/Jupyter and run the cells interactively.

    Reproducing results:

        Scripts and functions are provided to generate all cycles and tables as reported in the paper.

        See comments in the code for usage examples.

Reference

If you use this code in your research, please cite:

    John V. Teixido, "The Prime Vortex Sequence," 2025.

Data/Code Availability

All code and computational data needed to reproduce the results in the paper are available in this repository.

License

This project is licensed under the Apache 2.0 License. See LICENSE for details.

Contact

For questions or suggestions, please contact:
John V. Teixido
jvteixido@liberty.edu
