![Made with Qiskit](https://img.shields.io/badge/Made%20with-Qiskit-blue)
![Status](https://img.shields.io/badge/Project-Experimental-orange)
[ ![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.15203082.svg)](https://doi.org/10.5281/zenodo.15203082)
## Project Structure
˫Leaking information from black hole.ipynb

˫Readme.md

˪images/




A conceptual quantum simulation inspired by black hole physics.

## Overview:

This project explores the possibility of recovering structured information from Hawking Radiation emitted by black holes, using quantum circuits
and time reversal. By simulating black hole evaporation with upto 24 qubits (will try with more qubits), I aim to investigate the potential of quantum time reversal processes for information recovery. The project uses **Qiskit** to simulate quantum system.


We entangle them, create noise to mimic black holes and apply reversible transformation and noise - then compare measurement outcomes before and after reversing time using KL divergence (relative entropy). The goal is to investigate if information can be recovered or traced, simulating how it might behave near a black hole's boundary.

## Motivation:

In the 1970s, Stephen Hawking proposed that black holes emit thermal radiation, which seemed to destroy information - violating quantum theory. However, later developments like the Holographic principle, Ads/CFT, and Hawking's revised 2014 stance suggests that radiation may only appear random - and that information could be preserved, just highly scrambled.

This simulation is a conceptual step toward testing that idea on a quantum computer.

## Approach:

1.Create a Bell state to simulate entanglement between interior and radiation.

2.Introduce quantum noise to mimic decoherence.

3.Apply reversible operations (X and Z gates) to simulate "time reversal".

4.Use KL divergence to compare probability distributions before and after.

5.Visualize using Qiskit tools.


## What's Inside:

1.Leaking_information_from_black_hole.ipynb: Full simulation code in Qiskit'

2.Qubit circuit diagram + histogram visualization.

3.Relative entropy calculation to analyze reversibility and information preservation.

## New development (After trying with more qubits):

1. As the system scales up, the difference in structure between the post and reversed states vanishes or becomes too small to detect using KL Divergence.

2. Beyond a certain complexity, time reversal may not effectively distinguish between original and radiated information.

3. At lower qubit counts (6-20), there's a small but consistent structure preservation via reversal and at higher counts (20+), the reversal process becomes indistinguishable from noise - entropy saturates.

4. *My conclusion on this:*
    There exists a complexity threshold beyond which information in Hawking radiation becomes unrecoverable even with time reversal. 
   
5. But still this research is in progress so there is a space for improvement.

## Disclaimer:

This is a conceptual simulation, not a physical model of black hole radiation. It is meant to explore ideas related to information flow, quantum enatanglement, and scrambling, inspired by the black hole information paradox.

## License
This project is shared for educational and conceptual purposes. Not for commercial use.