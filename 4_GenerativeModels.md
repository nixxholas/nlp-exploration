## Generative Models, A Supervised learning model.

First, we'll have to find out what are supervised learning problems.
#### Supervised learning problems
- We have a set of predefined examples.
- We will then map inputs to the labels with the function of the model.

In the Part-Of-Speech (POS) tagging,
> Each training example consists of a sentence (the input) and the entire tag
sequence is the associated symbol (i.e. \NN).

> Thus, the function will take in a sentence and tags the input/s with
the tag sequence.

The first model to consider for supervised learning is the **Conditional Models**.

**!REMEMBER! EVERY 'p' MEANS PROBABILITY.**

#### Conditional Models
A conditional model is a discriminative model

Formula:
>  **p(y|x)** ----> p, Y given X

You can learn more about it [here](https://cs.stackexchange.com/questions/16777/hidden-markov-model-in-tagging-problem).

#### Generative Models
Compared to Conditional Models, the Generative model uses a different approach.

Formula:
> Distribution **p(x, y)** ----> A joint distribution,

Instead of expecting an input (in Conditional models, x has to be given). So thus,
 we will end up with this:

> **p(x, y) = p(y)p(x|y) / p(x)** which will then result in **p(y|x)**

So that's all for the sketchy formula that we need to know. Quite hard to digest?
I'll do a better explanation in the next chapter as we go through the Hidden Markov Model which is an iteration of the Generative Models.

##### [Back to main](https://github.com/nixxholas/nlp-exploration/)
