The starting weights are random but the deep learning agent updates them each step in the direction of the gradient which is most likely decided by the results of its actions and little by little they get better results due to more optimized weights. For example, say the results of current strength, is elimination of cat but it just wants to pick up the cat, then the gradient would be towards the direction which would lower the force used to pick up the cat. Each step would then decrease the force till it no longer is able to pick up the cat and the gradient reverses. 


This in more detail can be broken down into the following from [[3Blue1BrownNeuralNetwork_node2]]:

My first instinct tells me to do [[Newtons square root method]]

Second idea is maybe we can increase the amount of outputs. What effect would that have on the difficulty?

Is it necessary for it to be smooth can't we convert a non smooth output to a smooth one?, squeezing in some form?? That shouldn't be possible but who knows? Of course, all values won't be mapped but that doesn't matter!

Gradient = 0 -> local minimum.
Notes:
- Imagine a function with one input and one output
- Each slope check the direction wanted of the output and move the input towards that direction.
- Ball rolling down a hill, generalizes from single input to x, y
- Global minimum very difficult.
- What's the down hill direction?
- Gradient of a function gives you direction of steepest increase, take negative!
- Very important for output to be smooth
- Instead of converting inputs to direction one can convert them into relative importance. One way of saying that z = 3x + y gradient is [3, 1] is that the effect on z is 3 times bigger by x than by y.
- [[Backpropagation]] goes into the more detailed version

An algorithm commonly used in this endeavour is [[backpropagation]].