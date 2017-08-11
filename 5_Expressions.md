## Hidden Markov Models (HMM)

### Before we move on, why HMM rather than the other options available?
- [Comparisons with various POS tagging](http://dspace.bracu.ac.bd/jspui/bitstream/10361/83/1/Comparison%20of%20diffferent%20pos%20tagging%20techniques.pdf)

The evidence provided above proves that HMM works with our use case as a viable replacement to support and understand multiple languages for further processing.

So in the Hidden Markov Model (HMM), the previous chapter has explained that this is an iteration of a generative model. So first off, let us understand how a sentence is first processed in HMM.

We have an input sentence,
> Dory is a fish

Which will then have a tag sequence.
> Dory /JJ is /NN a /NN fish /NJ

**Note that these tags are random.. and is just a fake tag for this example.**

Thus from Topic 3, we have pull part of the formula's logic here.

Let the input sentence be x and the tag sequence be y.

Therefore, x and y will be,
> x = (Dory (x1), is (x2), a (x3), fish (x4))

> y = (JJ (y1), NN (y2), NN (y3), NJ (y4))

Which allows us to carry out the calculation of the probability of this HMM
instance into:

> arg max p(x1, ...., xn, y1, ...., yn)


### Trigram Hidden Markov Models (Trigram HMMs)
The simplest form of explanation for the core understand of Trigram HMMs have to
be watched here. [![Video Link](http://i3.ytimg.com/vi/98TARXun1xA/hqdefault.jpg)](https://youtu.be/98TARXun1xA?list=PLO9y7hOkmmSGSJA8S3gTigcyNDVJ31LLt&t=150)

After understanding what a Trigram HMM is, the input sentence and tag sequence has changed.

Input sentence, **(SAME)**
> Dory is a fish

Tag sequence.
> Dory /JJ is /NN a /NN fish /NJ /STOP

Notice that STOP has been added in a Trigram HMM to mark the end of a sentence. To convert a sentence given into the formula, it will look like:

Following the video's sample sentence, 'the dog laughs', we will have
> p(x1, ...., xn, y1, ...., yn) = q(D|*,*) x q(N|*,D) x q(V|D, N) x q(STOP|N,V) x e(the|D) x e(dog|N) x e(laughs|V)

Notice the D, N, V and STOP are tag sequences. (For the HMM example we gave earlier above, we have JJ, NN, NN and NJ and STOP)

##### [Back to main](https://github.com/nixxholas/nlp-exploration/)
