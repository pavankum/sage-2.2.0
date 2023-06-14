# ForceBalance inputs and outputs

The training targets used in this iteration (2.2.0) are identical to those in version 2.1.0. The scripts for dataset curation and ForceBalance inputs generation can be accessed from the following GitHub repository: https://github.com/openforcefield/sage-2.1.0.

During the optimization process, convergence was not achieved in the initial attempt. Therefore, we continued the optimization from the end of the first fit (fit1) using the `optimize.sav` file. This file contains the necessary `mvals` (mathematical values) to resume the optimization. Subsequently, convergence was successfully achieved in the second fit (fit2).

Both fits utilized the targets stored in the compressed directory targets.tar.gz. Within each directory, you can find the inputs of the ForceBalance run such as the initial force field file and the optimization setup, and the outputs of each run.
