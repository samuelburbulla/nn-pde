# Solving PDEs with neural networks

Neural networks can be used to solve partial differantial equations!
This repository is supposed to be a collection and playground for several such examples.


## Basic concepts
- The numerical solution of the PDE is represented by a neural network which maps coordinates to the solution value at this point.
  For instance, a single-layer perceptron with tanh activation function can be used which is a universal approximator.

- The PDE and its boundary conditions are incorporated within the loss function. We make use of pytorch's autograd functionality to compute the derviatives of the solution function with respect to its inputs.

- Standard optimization techniques are applied to fit the neural network to the solution of the PDE.


## Examples

 1. One-dimensional Poisson equation with Dirichlet boundary conditions and source term (see `poisson.ipynb`)
