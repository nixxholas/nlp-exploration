## Expressions

### What are expressions?

Expressions can be in the form of a few cases:
- Time expressions, where a phrase is being converted into a computational time format, be it a specific time or a range-based time set.
- Named entities, where words such as Coke can be named/categorized as a drink
- There is more cases where you'll be able to see online but we will only be going through the two as stated above.

##### Sample
Date of sentence: 1 Aug 2017

We have an input sentence,
> What do I have tomorrow?

Which will then have a time expressions
> What do I have **tomorrow**?

**The word "tomorrow" will be recognized by a time expression algorithm which would then be able to convert it into a computationally readable format:**

#### 1 Aug 2017 00:00 - 1 Aug 2017 23:59

This data retrieved is now able to be processed by any code.

Now the question is, how does it work?

**Due to the complexity of the algorithm developed, the github source code is linked below, which will then require you to do a step debug in order to learn the process of time expression recognition.**

The algorithm/engine that has been developed is segregated into the following sections:
- Tagging (To tag and ignore words that are not relevant to a time expression within the current context)
- Handlers (Converts tokenized words into its relevant time expression)
- Scanners (To scan for contexts, i.e. Timezones etc.)
- General processors such as a Numerizer, Tokenizer, Normalizer
- Registry

### The process
1. Sentence retrieval (The sentence is retrieved by the parser engine)
2. Tokenization (The sentence is simplified from a short conversation format to a grammatically corrected format)
3. Scanning (Scans the entire sentence and tags it with the proper computational number)
4. Handling (Handlers will convert the tokenized sentence into time if there is any)
5. Done!

#### [Time expression repository]()

##### [Back to main](https://github.com/nixxholas/nlp-exploration/)
