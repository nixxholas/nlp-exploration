## The Tagging Problem

Instead of diving deep into the explanation of the problem, we'll go through two
examples of the tagging problem first. (In the english language first of course.)

#### Problem 1, Part-Of-Speech (POS) tagging
**Sample Data:**
> Natural language processing

**Output:**
> Natural \JJ language \NN processing \NNJ

>[Tag your sentences here!](http://parts-of-speech.info)

From the tags given, we can tell that "Natural" is an adjective (JJ is a tagging
for a noun with the Part-Of-Speech tagger by Stanford U.) in this sentence while the word
"language" is a noun (\NN). Each word is given a tag. However, the problem with POS
 is that every word **may have more than a tag** where it can be a verb or also a noun.

#### Problem 2, Named Entity Recognition (NER)
Because NER does not have a fixed tagging example that can be reused commonly,
I've included the [stanford slides here](https://web.stanford.edu/class/cs124/lec/Information_Extraction_and_Named_Entity_Recognition.pdf)
for further use so that you'll be able to ideate your own set of named entities
in order to minimize the friction in understanding NER.

In short, NER is a way for us to tag common words categorized in our own way (i.e. Canon, Nikon & Fujifilm are named as a Brand entity.). That way, we will be able to distinguish non-official english words with our own recognition.

### Core constraints in Tagging Problems
The easier way is to [watch to this part of a video](https://youtu.be/kHvoHUGUitQ?list=PLO9y7hOkmmSGSJA8S3gTigcyNDVJ31LLt)
that will guide you through on how tags can come about to solve a conflict (When
a word can be a verb or also a noun).

#### You're done with understanding what we're going to solve now!

With POS tagging and NER, we will be able to recognize the words in a programatic way which would then allow us to further process the information.

### [Next Chapter](https://github.com/nixxholas/nlp-exploration/blob/master/4_CreatingAPOSTagger.md)

##### [Back to main](https://github.com/nixxholas/nlp-exploration/)
