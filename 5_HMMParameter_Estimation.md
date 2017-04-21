## Hidden Markov Model Parameter Estimation
The meaning of parameter estimation in HMM's context is to estimate the q and e
parameters from a set of training examples (These examples are learned by the model.) which we have seen in the formulas from the previous chapter, which are the trigram parameters and emission parameters respectively.

**In overall for this topic, we will be using estimation with the Hidden Markov Model for learning.**

[Click here if you want to learn basic smoothing (Smoothed Estimation)](http://www.cs.jhu.edu/~jason/465/hw-hmm/hw-hmm.pdf)

**The main reason why HMM's name was given is partially because:**

## The word "Hidden" was used as HMM supports learning with a hidden state.

#### When learning without a hidden state,

![Learning without a hidden state](/Images/5_LearningWithoutHiddenState.png)

> Learning will be simple since we know the correct path for each sequence in our training set. We would then estimate parameters by counting the number of times each parameter is used across the training set. (Dewey, 2017)

#### However,

![Learning with a hidden state](/Images/5_LearningWithHiddenState.png)

> if we don’t know the correct path for each sequence in our training set, consider all possible paths for the sequence. We then estimate parameters through a procedure that counts the expected number of times each transition and emission occurs across the training set. (Dewey, 2017)

#### This is also known as Learning with a Hidden State.

But before we're able to learn with hidden states, let's look through what learning parameters are first.

**If we know the state path for each training sequence, learning the model parameters is simple**
- No hidden state during training
- Count how often each transition and emission occurs – normalize/smooth to get probabilities
- Process is just like it was for Markov chain models

**If we don’t know the path for each training sequence, how can we determine the counts?**
- key insight: estimate the counts by considering every path weighted by its probability

### Learning Parameters with The Baum-Welch Algorithm
##### a.k.a The Forward Backward Algorithm.


**About The Baum-Welch Algorithm**
- it is an Expectation-Maximization (EM) Algorithm.

> EM is a family of algorithms for learning probabilistic models in problems that involve hidden state and is generally used to find maximum likelihood estimates for parameters of a model (Dewey, 2017)

In this context, the hidden state is the path that explains each training sequence

### Sketching your Algorithm

![Sketching your algorithm slide](/Images/5_SketchingAlgo.png)

#### The Expectation Step

Formula:
> ### Pr(πi =k|x)
* i is the base of π.

First, we need to know the probability of the 'i' th symbol
being produced by state k, given sequence x. Given this we can compute our expected counts for state transitions, character emissions. (Dewey, 2017)



##### References
Dewey, C. (2017). Hidden Markov Model Parameter Estimation. 1st ed. [ebook] Madison, Wisconsin, U.S: University Of Wisconsin-Madison. Available at: https://www.biostat.wisc.edu/bmi576/lectures/hmms-parameter-estimation.pdf [Accessed 20 Apr. 2017].
