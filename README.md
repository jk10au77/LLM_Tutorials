# LLM_Tutorials
Large Language Models tutorials
-------------------------------------------------------------
https://developers.google.com/machine-learning/resources/intro-llms#what_is_a_language_model

https://developers.google.com/machine-learning/crash-course/prereqs-and-prework

Learning Objectives
----------------------------------------------------------
a. Define language models and large language models (LLMs).
b. Define key LLM concepts, including Transformers and self-attention.
c. escribe the costs and benefits of LLMs, along with common use cases.
----------------------------------------------------------

What is Language Models?
-----------------------------
a. Language model is a machine learning model that predicts and generates credible language
    AutoComplete language is Language model
b. These models work by estimating the probability of of a token or a sequence of tokens occuring within a longer sequence of tokens

Consider the following sentence:
--------------------------------
When i see a vehicle standing on the highways,My first thought would be that ----------------

If you assume that a token is a word, then a language model determines the probabilities of different words or sequence of words to replace that underscore

For the above example: A language model might replace with the following probabilities.
a. animals might be crossing the road 3.4%
b. there might be accident   2.6%
c. there might be some road maintence 10.8%
....

Note:
------
a. A 'sequence of tokens' could be an entire sentenceor a series of sentences. 
b. i.e a Language model could calculate the likelihood of different sentences or blocks of text.


What is a Large Language Model?
------------------------------------
a. Modelling a human language is a highly complex and resource-intensive tasks.
b. As models are built bigger and bigger, their complexity and efficacy increases. 
c. Early language models could predict the probability of a single word;
d. modern large language models can predict the probability of sentences, paragraphs, or even entire documents.
e. The size and capability of language models has exploded over the last few years as computer memory, dataset size, and processing power increases, and more effective techniques for modeling longer text sequences are developed.

How large is large?
----------------------------
a. Large is used to describe the BERT (110M parameters) as well as PaLmM (upto 340B parameters)
b. "Large" can refer either to the number of parameters in the model, or sometimes the number of words in the dataset.

Parameters:
--------------
a. are the weights the model learned during training
b. are used by models to predict the next token in the sequence 

Transformers:
---------------
a. It ws introduced in language models in 2017.
b. It is an architecture designed aroung the idea of attention.
c. It processes longer sequences by paying attention on the most important part of input
d. It also solves memory issues faced in the earlier models.
f. It is the state-of-art architecture for a wide range of language model applications, such as translators.
g. Full transformer consists of 
    i.   an encoder - converts the input input text into an intermediate representation, and
    ii.  a decoder - converts the intermediate representation into useful text.

Self-attention:
----------------
a. Transformer mainly rely on the 'self-attention' concept
b. The self 'self' part of the 'self-attention' refers to the 'egocentric'. i.e. it focuses on the each token of the input corpus.
c. On behalf of each token of input, the 'self-attention' asks, 'What is the impact of every token of the imput matter to me'. 

For example:
--------------
Consider the following sentence:

I can not go outside the house because it is raining.

The sentence contains 11 words. So each word is paying attention to the other 10 words. Then it evaluates the impact of these 10 words have on me. 
For example, notice that the sentence contains the pronoun it. Pronouns are often ambiguous. The pronoun it always refers to a recent noun, but 
in the example sentence, which recent noun does it refer to: the animal or the street?
The self-attention mechanism determines the relevance of each nearby word to the pronoun it.


What are the use cases of LLMs?
--------------------------------
a. LLMs are excellent in mimicking human speech patterns
b. They are emergent abilities. LLMs can even solve some math problems and write code.
c. LLMs can be components of models that do more than just generate text. 
d. Recent LLMs have been used to build sentiment detectors, toxicity classifiers, and generate image captions.

LLMs considerations. i.e. When to consider LLMs?
-------------------------------------------------
a. Large LLMs are expensive. They can take months to train, thus they consume large resources.
b. Engineering challaenges arise because of the fact that that these LLMs are built upon large number of parameters ranging from BERT (110M Parameters) to PaLM (340B Parameters)
   Special Infrastructure and Programming language are required to coordinate the flow of information to chips and back again.

        Then the question is to how to mitigate theese costs of these LLMs
        -------------------------------------------------------------------
        There are two ways 
            a. Offline interference 
            b. Distillation
c. Bias is another problem in LLMs and should be considered in training and deployment.
d. When trained on human languages, these LLMs can introduce potential ethical issues such as misuse of language, and bias in race, gender, color, relion, etc.
