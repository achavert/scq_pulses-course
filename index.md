---
title: Home
layout: index
---
 
## Pulse-level control at Qmio with OpenPulse

Quantum Computing uses the properties of quantum systems to perform operations under a new logic paradigm. These operations, called quantum gates, are abstract linear operations on qubit spaces, and by composing them, we can build quantum algorithms to solve problems in a different way to the classical solutions. In reality, we need to encode the qubits on real physical systems (transmons, trapped ions, cold atoms...) and their quantum gates will represent specific processes performed over them, like applying magnetic fields, lasers, etc. <br>
<br>
On this course, we'll learn how Qmio physically implements its quantum gates through microwave pulses. Starting from the superconducting qubit formulation, and understanding how pulses perform these operations, we'll see how to develop experiments at pulse-level in Qmio with the OpenPulse grammar from OpenQASM.  


## Setup
First, to access the Qmio CPD nodes at CESGA (through a @qmio.cesga.es account) type:

```ssh <user>@qmio.cesga.es```

or

```ssh -m hmac-sha2-512 <user>@qmio.cesga.es```

Request a ```compute``` node.<br>

Run the following comands:

```
module load qmio/hpc gcc/12.3.0 pytket/1.23.0-python-3.9.9 qmio-run/0.5.1-python-3.9.9 
module load qiskit/1.2.4-python-3.9.9 qmio-tools/0.2.1-python-3.9.9
jupyter notebook --ip=$(hostname -i) --port=8889 &> opa.out &
cat opa.out
```

Copy the first link printed and paste it on your browser. Now you are ready to execute the notebooks of this course, you can find them in the ```\notebooks``` folder from this repository.


## Contents

This course is composed of four notebooks that explain the superconducting qubit system and its control at pulse level. Oriented to understand how the native quantum gates are physically implemented, and to be able to design experiments in Qmio. Also, it includes a revised documentation of the OpenPulse grammar, specifically for Qmio's available features, and a more in depth dive into the theory of pulse control.  

### Presentation

[Link to the slides](https://www.canva.com/design/DAHBdmQNDFE/8PaGsgNXGk9oKSen7-YmTQ/edit?utm_content=DAHBdmQNDFE&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

## References and acknowledgements

This course was produced as part of the QUORUM SPAIN project at the Galician Supercomputing Center (CESGA).<br>
<br>
QUORUM SPAIN is a project funded by CDTI and financed with funds from European Union Next Generation through the Recovery, Transformation and Resilience Plan.

