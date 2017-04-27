## Topic 1: Basics of Natural Language Processing (NLP) for Instant messaging conversations

**Before we begin, please understand that the information below is redundant in relation to the rest of the other topics and is just a simple explanation towards NLP. Reading this page is recommended to help you in understanding how NLP exactly works.** (Skip this if you do know how it works.)

### NLP is segregated into two components.
- **Natural Language Understanding** and,
- **Natural Language Generation**

##### Natural Language Understanding Involves:
 - Mapping the given input in natural language into useful representations.
 - Analyzing different aspects of the language.

**In short, NLU is the way a language is supposed to be understood in.**

##### Natural Language Generation Involves:
1. **Text Planning** - Involves retrieving relevant content from a set of data.
2. **Sentence Planning** - Involves the creator to create a dataset (Can be a
word, phrase or sentence.) that is self defined in order to analyze and
retrieve relevant content from a data (Or in this case, a sentence).
3. **Text Realization** - Involves mapping a sentence's plan into a structure.

###### These two components make up the core principles of NLP.
However, what we will be doing requires focusing on the key principles on NLU first. Thus, here's a little snippet of what will come upon us.

**First and foremost, NLU is more complex than NLG because of its nature of ambiguity (it is open to or having several possible meanings or interpretations; equivocal).**

**NLU is an input of language into a computer while NLG is an output of language from a computer.**

Hold up, I will explain to you about the underlying problem now.

NLU has a core level of complexity and due to this nature, we have several levels of ambiguity.
- **Lexical Ambiguity** - In this instance, a language that has lexical ambiguity means there are two or more possible meanings within a single word.
- **Syntax-Level Ambiguity** - In this instance, a language that has syntax-level ambiguity has several forms of sentences that can produce the same type of meaning (Or can be parsed in different ways).
- **Referential Ambiguity** - In this instance, a language that has referential ambiguity means that words can have reference to something. (i.e. I am done with my work.) -> Who is I? or in another way, who is done with his work?

With these 3 levels of ambiguity, we can deduce that English has all 3 levels and is complex. Thus, One input can contain several meanings while many inputs can contain the same meaning (Many to Many in a ERD).

Okay.. So now that we're done with the explanation of what is the hurdle in NLU, here's a flow of how a sentence is processed in NLP.

![NLP Process Diagram](https://www.tutorialspoint.com/artificial_intelligence/images/steps_in_nlp.jpg)

[(Steps in NLP, 2017)](https://www.tutorialspoint.com/artificial_intelligence/images/steps_in_nlp.jp)

I'll be quoting from [tutorialspoint](https://www.tutorialspoint.com/artificial_intelligence/artificial_intelligence_natural_language_processing.htm) (with some simplified) for the basic explanation of each step.

**Lexical Analysis**
> This Involves using a lexicon of a language (In a way, a dictionary of that language. Or the collection of words and phrases in a language) to divide text information into paragraph/s, sentence/s or word/s.

**Syntactic Analysis**
> Involves analysis of words in the sentence for grammar and arranging words in a manner that shows the relationship among the words. The sentence such as “The school goes to boy” is rejected by English syntactic analyzer. ([www.tutorialspoint.com. (2017)](https://www.tutorialspoint.com/artificial_intelligence/artificial_intelligence_natural_language_processing.htm))

**Semantic Analysis**
> It draws the exact meaning or the dictionary meaning from the text. The text is checked for meaningfulness. It is done by mapping syntactic structures and objects in the task domain. The semantic analyzer disregards sentence such as “hot ice-cream”. ([www.tutorialspoint.com. (2017)](https://www.tutorialspoint.com/artificial_intelligence/artificial_intelligence_natural_language_processing.htm))

**Discourse Integration**
> The meaning of any sentence depends upon the meaning of the sentence just before it. In addition, it also brings about the meaning of immediately succeeding sentence.

**Pragmatic Analysis**
> During this, what was said is re-interpreted on what it actually meant. It involves deriving those aspects of language which require real world knowledge.

For further understanding of each step, here's the [link](https://www.tutorialspoint.com/artificial_intelligence/artificial_intelligence_natural_language_processing.htm) to it.

**So.. How do we implement NLP in Instant Messaging contexts? Let's learn what the solution solves first.**

### [Next Chapter](https://github.com/nixxholas/nlp-exploration/blob/master/2_BasicsOfLanguageModels.md)

##### [Back to main](https://github.com/nixxholas/nlp-exploration/)

###### References
Steps in NLP. (2017). [image] Available at: https://www.tutorialspoint.com/artificial_intelligence/images/steps_in_nlp.jpg [Accessed 18 Apr. 2017].
www.tutorialspoint.com. (2017). Artificial Intelligence Natural Language Processing. [online] Available at: https://www.tutorialspoint.com/artificial_intelligence/artificial_intelligence_natural_language_processing.htm [Accessed 18 Apr. 2017].
