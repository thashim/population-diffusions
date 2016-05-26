# Overview
Code and paper repository for the ICML paper "Learning population level diffusions with generative recurrent networks"

# Paper

Tex and PDF of the paper are in the root directory.

# Code

The codebase consists of four files:

1. **Theano-functions** contains the main inference methods, loss functions, hyperparam optimizers.
2. **Theano-test** runs the simulation datasets
3. **Single-cell-stuff** runs the single-cell rnaseq experiments
4. **Flow-functions** is a non-theano version of the inference methods (deprecated, not used to generate results) and some plotting functions used in single-cell plots.

# Usage

To use on your own machine, modify theano-functions to write to your own .theanorc (currently writes to /cluster/thashim).

Additionally, for the single-cell data, wget the data from [GSE65525](http://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE65525) and put it in a directory named `rnase' one level below. The second code block in single-cell-stuff shows expected output.
