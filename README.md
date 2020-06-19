# Parity Models
This repository contains the code used for developing and evaluating parity
models. A parity model is a computational unit that enables the use of ideas
from erasure coding to impart resilience against slowdowns and failures that
occur in distributed data processing and serving environments.

This repository focuses particularly on using ideas from erasure codes to
impart resilience to prediction serving systems performing inference with
neural networks. For a brief overview of how a parity model enables this
resilience, please see this [description](train/README.md). We will add a
broader explanation of the function of a parity model to this README in the
near future.

This repository originated as the artifact associated with the SOSP 2019 paper
[Parity Models: Erasure-Coded Resilience for Prediction Serving Systems](https://dl.acm.org/doi/10.1145/3341301.3359654).
It has since evolved beyond serving this paper in isolation. The original
artifact associated with the SOSP 2019 paper is located in the
`sosp2019-artifact` branch.

## Repository structure
* [train](train): Code for training a neural network parity model
* [clipper-parm](clipper-parm): Code for ParM, a prediction serving system that
employs parity models to impart erasure-coding-based resilience to slowdowns
and failures.

Please see the READMEs in each of these subdirectories for more details.

## Cloning the repository
If you are only interested in the training portion of the repository, you
can clone the repository as:
```bash
git clone https://github.com/Thesys-lab/parity-models.git
```

If you are intersted in running ParM, the prediction serving system employing
parity models, you will need to clone required submodules using the
`--recursive` flag:
```bash
git clone --recursive https://github.com/Thesys-lab/parity-models.git
```

## License
```
Copyright 2019, Carnegie Mellon University

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

## Support
We graciously acknowledge support from the National Science Foundation 
(NSF) under grant CNS-1850483 and an NSF Graduate Research Fellowship 
(DGE-1745016 and DGE-1252522).
