Back propagation computes the gradient using the chain rule at nodes leading up to the output.
This gradient reflects the sensitivity at which that node affects the value of the output. 
By first doing a forward pass, you can compute the loss and the values of each individual node, which can then be used during back propagation to find the gradient. 
By going in the opposite direction of these gradients at a certain magnitude (step size), you can minimize a loss function and train a neural net for accuracy by executing a forward pass, back propagation, and training step (and repeat).
Note that gradients accumulate, so resetting gradients in between loops is necessary. 