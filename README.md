# Physical-Informed-NN
Inverse-Problems Project PINNS - ErSE 213

This is the repository that contains the experiments related to the implementation of  physical informed deep learning models.
We decided to implement three problems that increases their complexity and show the capabilities of this kind of framework to
handle system identification from the perspective of solving and infering the parameters of differential equations.

Problems:

1. Harmonic Oscillator - RLC circuit: we simulated an over-dumped case for this problem. 1 dimensional (only time) problem
2. Burgens Equation: A 2d case -- 1 spatial and 1 temporal dimension.
3. Navier-Stokes: A 3d case -- 2 spatials and 1 temporal dimension. This we used the deepXDE library in order to stabilize the traning of the model

From the implementaion we identiy that we can learn the dynamics of the system without much effort (besides a correct model description). So, for the
cases where we do not have data available, we can use the physic of deep problem to act as regularization and learn the dynamics of the overall system.
Besides that, the physics and data can help each other in the sense we can use both to learn a better solution in the parameter space in order to find
a good set of parameters that mimics the desired dynamical system. 
