# ForceBalance inputs and outputs

The training targets used in this iteration (2.2.0) are identical to those in version 2.1.0. The scripts for dataset curation and ForceBalance inputs generation can be accessed from the following GitHub repository: https://github.com/openforcefield/sage-2.1.0.

The targets utilized in the fit were stored in the compressed directory targets.tar.gz. The inputs of the ForceBalance run such as the initial force field file and the optimization setup, and the outputs of each run.

- `forcefield/` : Contains the initial force field to start the optimization from.
- `optimize.in` : ForceBalance optimization input file that contains the target and hyperparameter definitions.
- `result/`     : Contains the final optimized force field file.
- `output_of_optimization.tar.gz` : Compressed text file which has the forcebalance run log.
- `targets.tar.gz` : training targets used in the force field fits.
