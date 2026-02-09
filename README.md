---
title: Home
layout: index
---
 
# Pulse-level control at Qmio with OpenPulse

A practical introduction to pulse-level control of superconducting qubits with the OpenPulse and Qmio's implemented features.


## Setup
Access the Qmio CPD nodes at CESGA (through a @qmio.cesga.es account):

```ssh <user>@qmio.cesga.es```

or

```ssh -m hmac-sha2-512 <user>@qmio.cesga.es```

Request a ```compute``` node.<br>
<br>

Run the following comands:

```
module load qmio/hpc gcc/12.3.0 pytket/1.23.0-python-3.9.9 qmio-run/0.5.1-python-3.9.9 
module load qiskit/1.2.4-python-3.9.9 qmio-tools/0.2.1-python-3.9.9
jupyter notebook --ip=$(hostname -i) --port=8889 &> opa.out &
cat opa.out
```

Copy the first link returned and paste it on your browser. You are ready to execute the notebooks on this course, you can find them in the ```\notebooks``` folder in this repository.


## Contents

This course is composed of four notebooks that explain the superconducting qubit system and its control at pulse level. Oriented to understand how the native quantum gates are physically implemented, and to be able to design experiments in Qmio. Also, it includes a revised documentation of the OpenPulse grammar, specifically for Qmio's available features, and a more in depth dive into the theory of pulse control.  


### Notebooks
- [1. **Introduction to qubit physics**](/content/notebook01.md)

- [2. **Single-qubit driving**](/content/notebook02.md)

- [3. **Qubit spectroscopy**](/content/notebook03.md)

- [4. **Two-qubit driving**](/content/notebook04.md)

### Documentation
- [OpenPulse grammar documentation for Qmio](/content/notebookE1.md)

- [Transmon and pulse-level control theory](/content/notebookE2.md)


## References and acknowledgements
This course was produced as part of the QUORUM SPAIN project at the Galician Supercomputing Center (CESGA).<br>
<br>
QUORUM SPAIN is a project funded by CDTI and financed with funds from European Union Next Generation through the Recovery, Transformation and Resilience Plan.

