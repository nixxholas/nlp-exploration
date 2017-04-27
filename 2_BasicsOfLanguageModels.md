## Topic 2: Basics of Language Models

#### A language model is a form of speech recognition system used by NLP for a certain language.

### In a basic form of a language model, we can find the probability by:
> P(|W| = 4, w1 = "hi", w2 = "this", w3 = "is", w4 = "Nicholas")

Where W is the language model.
**Note** -> w0 is a start tag to signalize the start of the sentence.
**Same goes for w5 as an end tag to signalize the end of the sentence.**

#### By using Incremental Computation, we'll have an equation:
![ICEquation](/Images/2_IncrementalComputationEquation.png)
That looks confusing. So the main point is, how do we get the probability?

##### We'll compute the probability by what's called the:
## Maximum Likelihood Estimation (ML Estimation).

![Maxmimum likelihood basic equation](Images/2_MaximumLikelihoodBasicEquation.png)

W is the sentence that we're analyzing.

In this example:
> **##Start## This is Nicholas ##End##**

Let's say i = 2, this means that we're accessing "is".

> **P(is | ##Start## This) = C (##Start## This is) / C (##Start## This)**

C (aka Count) is equal the number of times this word has appeared with the machine.

This is the resultant equation we will get.

An example of a simple algorithm is a Naive method, which returns 0 if the data that we have does not match with the sentence given. ([Extra Video Tip](https://www.youtube.com/watch?v=M3uA0dSNI98&list=PLO9y7hOkmmSH7-p6que1MYbhBx74AzH7-&index=2))

#### However, such an equation will result in weak probabilities when the counts are low.
- Unknown words will often be ignored

Thus, we have the **Likelihood** Probability to increase model accuracy.

![Likelihood equation](Images/2_LikelihoodEquation.png)

**NOTE** ->  [What does ∏ mean?](https://math.stackexchange.com/questions/620187/what-does-the-prod-symbol-mea)

-> ∈ means "an element of"

##### Before the confusing part comes, we'll go through the fundamentals of what we want to achieve in these topics, the Hidden Markov Model. ([Adapted from StackExchange](https://stats.stackexchange.com/questions/2457/markov-process-about-only-depending-on-previous-state))
#### You will have to google from this section all the way till the end. (Too many references to make, I will come back to this topic to add on when I'm done with school.)

[**Click here for extra Markov Chain Information**](https://webcourse.cs.technion.ac.il/236522/Spring2008/ho/WCFiles/class08-m8.pdf)

![Hidden Markov Chains](/Images/2_MarkovChains.png)

To further aid you into understanding what a first order Markov Chain is, here is an example.


- However, as the numbers calculated with likelihood are low, this may result in integer underflow. This can be resolved with **Log likelihood**.

![Log Likelihood equation](Images/2_LogLikelihoodEquation.png)

- This way, a high level of accuracy can be obtained while maintaining high levels of data integrity.

##### References
- mean?, W. (2017). What does the $\prod$ symbol mean?. [online] Math.stackexchange.com. Available at: https://math.stackexchange.com/questions/620187/what-does-the-prod-symbol-mean [Accessed 27 Apr. 2017].
