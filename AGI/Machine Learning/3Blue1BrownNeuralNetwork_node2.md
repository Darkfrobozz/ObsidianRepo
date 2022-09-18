Plan:
- Recap
- Gradient descent
- Analyze this network
- Where to learn more
- Research corner



Quick recap:
- Neurons are functions, they take in an input and they modify it with a weight and some bias. This modified version is the output
- These neurons are structured in layers, where they linked together input / output wise
- There are input neurons.
- The outputs are generally squeezed with some function so as to know that they are in a certain range.
- This is supposed to make them able to piece more and more segments together.


Finding minima?
Random init.
'cost' function, that tells them what is wrong. It could work in the way that the cost is really high when it is bad and low when it is good so the goal is to make it minimize cost or so to say find the minimum.

Huge input, small output


We need to tell it how to change and notes from this video are provided in the general knowledge of:
[[Gradient Descent]]

Ideas and questions:
- [[Backpropagation]] goes into the more detailed version


Answer:
- I could perhaps use the visual version to paint something!
- I could make a neural network for identifying edges then use that neural network to make one for identifying numbers and in such a way 'paint' the initialization.

Interesting that that the idea I had in [[3Blue1BrownNeuralNetwork]] is addressed here as wrong, basically saying that there is a rebuttal paper towards the idea that they are just memorizing the entire dataset. But it is a little confusing how they bring this up, I would like to take another look at this video again and rethink it:

https://www.youtube.com/watch?v=IHZwWFHWa-w

The idea as far as I can understand is that correctly labelled information is easier for a neural network to navigate.


