# nn-exploration
My past exploration into neural networks. Contains a train.csv file from the [MNIST dataset](https://en.wikipedia.org/wiki/MNIST_database).

Much of this project was spent teaching myself the theory. I did this project before I even knew what a derivative or a matrix was, so you can imagine how long that took!

## Naive implementation
This was my first implementation of a neural network, and there's a backstory.

### My naviety
I was in my early-to-mid years of high school making this, and I didn't know anything about
matrices or derivatives. After teaching myself derivatives (not matrices, I'll talk about that later),
and the concept of gradient descent, I set out to make my own implementation.

### My implementation's inefficiency
I actually used forward and not backward propagation. By forward propagation, I mean that, 
to perform gradient descent, I kept track of each gradient descent partial derivative separately 
and went forward through the network, summing the partial derivatives at the end.

I did this because I didn't know that you were meant to use backward propagation.
I only knew basic theory about derivatives and the concept of gradient descent, and tried to figure the rest out myself.

Furthermore, I didn't use matrices at all! I didn't know they existed, and I didn't 
know that you were supposed to, or even that you could mathematically represent a 
neural network using matrices.

Overall, this led to the long and clunky implementation that is naive_implementation.ipynb.

### Side note
I'm actually glad I did my neural network this way at first. 
It taught me a lot about neural networks and introduced me to matrices.

## Proper implementation
After realizing that I should have used bacakpropagation and matrices, I improved my understanding a ton,
and made a much more efficient implementation using numpy.

You can find that in proper-implementation.ipynb.
