# ARES (BASS) 2024

This repository contains the code for the paper "Systematic Analysis of Label-flipping Attacks against Federated
Learning in Collaborative Intrusion Detection Systems", published in the proceedings of the *19th International Conference on Availability, Reliability and Security* (ARES 2024).

If you use this code, please cite the following paper:

```bibtex
@inproceedings{lavaur_ares_2024,
  TITLE = {{Systematic Analysis of Label-flipping Attacks against Federated Learning in Collaborative Intrusion Detection Systems}},
  AUTHOR = {Lavaur, L{\'e}o and Busnel, Yann and Autrel, Fabien},
  BOOKTITLE = {{The 19th International Conference on Availability, Reliability and Security}},
  SERIES = {4th International Workshop on Behavioral Authentication for System Security (BASS)},
  ADDRESS = {Vienna, Austria},
  YEAR = {2024},
  MONTH = Jul,
  EDITOR = {ACM},
  URL = {https://hal.science/hal-04559018},
  DOI = {10.1145/3664476.3670434},
  KEYWORDS = {intrusion detection ; data-poisoning ; label-flipping ; backdoors ; systematic analysis ; quantitative assessment},
  HAL_ID = {hal-04559018},
  HAL_VERSION = {v1},
}
```

## Abstract

With the emergence of federated learning (FL) and its promise of privacy-preserving knowledge sharing, the field of intrusion detection systems (IDSs) has seen a renewed interest in the development of collaborative models.
However, the distributed nature of FL makes it vulnerable to malicious contributions from its participants, including data poisoning attacks.
The specific case of label-flipping attacks, where the labels of a subset of the training data are flipped, has been overlooked in the context of IDSs that leverage FL primitives.
This study aims to close this gap by providing a systematic and comprehensive analysis of the impact of label-flipping attacks on FL for IDSs.
We show that such attacks can still have a significant impact on the performance of FL models, especially targeted ones, depending on parameters and dataset characteristics.
Additionally, the provided tools and methodology can be used to extend our findings to other models and datasets, and benchmark the efficiency of existing countermeasures. 


## Usage

This repository contains the code used to generate the results presented in the paper.
Most of it consists of Jupyter notebooks that can be run in any Python environment, as all the associated data is included in the repository.

A `shell.nix` file is provided for Nix users to reproduce the exact environment used to generate the results.
This includes the correct dependencies, including the [`eiffel`](https://github.com/phdcybersec/eiffel) library, the evaluation framework used in this study.
For using the notebooks only, any Python environment with `pandas`, `scikit-learn`, and `matplotlib` should be sufficient.

If you wish to generate the results from scratch, or extend the study to other models or datasets, please refer to the [`eiffel`](https://github.com/phdcybersec/eiffel) repository for more information.

## License

This code is released under the MIT License. See the `LICENSE` file for more information.
The paper itself is licensed under the [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) license.