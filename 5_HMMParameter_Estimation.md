## Hidden Markov Model Parameter Estimation
The meaning of parameter estimation in HMM's context is to estimate the q and e
parameters from a set of training examples (These examples are learned by the model.) which we have seen in the formulas from the previous chapter, which are the trigram parameters and emission parameters respectively.

**In overall for this topic, we will be using estimation with the Hidden Markov Model for learning.**

[Click here if you want to learn basic smoothing (Smoothed Estimation)](http://www.cs.jhu.edu/~jason/465/hw-hmm/hw-hmm.pdf)

**The main reason why HMM's name was given is partially because:**

## The word "Hidden" was used as HMM supports learning with a hidden state.

#### When learning without a hidden state,

![Learning without a hidden state](/Images/LearningWithoutHiddenState.png)

> Learning will be simple since we know the correct path for each sequence in our training set. We would then estimate parameters by counting the number of times each parameter is used across the training set. (Dewey, 2017)

#### However,

![Learning without a hidden state](/Images/LearningWithHiddenState.png)

> if we don’t know the correct path for each sequence in our training set, consider all possible paths for the sequence. We then estimate parameters through a procedure that counts the expected number of times each transition and emission occurs across the training set. (Dewey, 2017)

#### This is also known as Learning with a Hidden State.

##### References
Dewey, C. (2017). Hidden Markov Model Parameter Estimation. 1st ed. [ebook] Madison, Wisconsin, U.S: University Of Wisconsin-Madison. Available at: https://www.biostat.wisc.edu/bmi576/lectures/hmms-parameter-estimation.pdf [Accessed 20 Apr. 2017].
