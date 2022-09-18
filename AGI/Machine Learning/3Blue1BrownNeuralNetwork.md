Comments on some crazy acceptance of our ability to distinguish some concept hidden in noise.


Goal: 
- Put together a neural network that can recognize digits.
- Plain vanilla - multilayer perceptron



[[Neural networks]] are inspired by brains, a neuron is simply according to 3Blue1Brown a holder for a digit.



Hidden layers - two hidden layers maybe with 16 neurons in total.

What is the hope of this specific example?
He explains this by humans are recognizing figures by connecting various simpler forms to them. He then goes into explaining that this is what we hope the neural network will do. 

Edges -> Forms -> Figures

/ side not I do believe that the real reason is that statistics is taken advantage of when you have multiple layers, say the likelihood of it being a 9 converges to the last neuron in the last layer through each layer.

[[Statistical theory]] is what I will call the previous side not.

This system uses edges between neurons and these edges have weights and these represent the strength of the activation of the neuron given a certain input. These strengths are then summed up to give us the input to the next neuron, which means we can filter away parts of the input with help of these links and focus in on some parts, if other neurons are doing the same we can later sum composite this.

A [[sigmoid function]] can be used to make the sums into valid inputs.


Neural Networks can be described with [[Linear algebra]]:

sigmoid(Wa^(0) +  b)

Now the more complicated version of a neuron is a function, taking in a parameter putting out a weighted output.

[[ReLU]] is more common now, this is inspired by the biology of neural networks, where the input has to pass a certain threshold.

This is according to 3blue1brown the structure but the learning process is account for in the next node [[3Blue1BrownNeuralNetwork_node2]] 

