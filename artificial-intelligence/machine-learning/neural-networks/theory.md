- A neural network (also `artificial neural network` or `neural net`, `ANN`, or `NN`) is a model inspired by the structure and function of biological neural networks in animal brains.
- A neural network is a special type of function that takes some inputs, performs some calculations on them, and returns an output.
- An ANN consists of `nodes` (artificial neurons) connected by `edges`. The nodes model the neurons in a brain, while the edges model the synapses in a brain.
- Each neuron receives signals from connected neurons. It processes them and sends a signal to other connected neurons.
- The `activation function` is a non-linear function that calculates the output of the node based on its inputs and weights.

**Parameters**
- Usually, parameters = `weights` + `biases`. As an example, in a uni-variate linear regression model `y = mx + b`, m is the weight and b is the bias. Bias is a weight that scales a constant input of 1.
- `Weights` determine the strength of the input and they are "learned".
- `Hyperparameters` are aspects of a model or optimization algorithm that cannot learned automatically. As such, their values must be decided on a priori by humans. Examples include the learning rate, the number of layers in a neural network, or the regularization technique(s) used during training.

**Markov chains vs neural networks**
- Markov chains relied on storing probabilities in tables.
- Neural networks use function approximation algorithms to calculate probabilities. These are generated algorithmically instead of being stored as a big table.

![neural_network.png](neural_network.png)

## References
- https://en.wikipedia.org/wiki/Neural_network_(machine_learning)
- https://en.wikipedia.org/wiki/Activation_function
- https://www.reddit.com/r/learnmachinelearning/comments/oq4mk0/comment/h6bq2jg/