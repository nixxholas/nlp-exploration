## Creating a Part Of Speech Tagger

#### Objectives
- Store a set of predefined examples for tagging.
- Utilize a Part Of Speech Tagging If logic to tag words.
- Filter out words that are "noisy" for us.

In the Part-Of-Speech (POS) tagging,
> Each training example consists of a sentence (the input) and the entire tag
sequence is the associated symbol (i.e. \NN).

> Thus, the function will take in a sentence and tags the input/s with
the tag sequence.

To simplify the process for creating a Part Of Speech tagger engine, we will segregate it into two segments:
- Corpus (This is simply known as a dictionary)
- Tag Processing Object (An object instantiated to process words, phrases or sentences by including a tag with each word.)

These two elements will create the core foundation of a Part of speech tagging engine, which can be expanded into greater uses such as:
- Word filtration
- Grammar checking or rather, linguistic correction

The github source code link below is an example of a simple part of speech engine that has been developed. This engine is able to recognize over 90000 characters/words within the English dictionary and uses the Brills English Corpus to recognize, identify and process data.

#### [View the source code here](https://github.com/nixxholas/nlp-postagging)

### [Next Chapter](https://github.com/nixxholas/nlp-exploration/blob/master/5_Expressions.md)

##### [Back to main](https://github.com/nixxholas/nlp-exploration/)
