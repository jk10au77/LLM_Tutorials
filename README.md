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

c. 
