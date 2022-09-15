# DeepQuantile
Deep Quantile Regression with tuning-friendly yaml file
Following Tansey's work at [here](https://github.com/tansey/quantile-regression)

Run the simultion by inputting `python python/benchmark.py` in command line/terminal

The simulation compares the result between mean-squared error net and deep quantile regression net.

Something to notice about the yaml file
1. Only SGD and Adam are currently available as an optimizer
2. `layer_specs` does NOT contain input and output dimension, it only contains hidden layers. So if don't want an MLP, just leave it as an `[]`
3. `L_1_weight` is different from `lambda`, former one refers to its weight compared to L-2 penalty, later one refers to the shrinking contant for either penalty.
