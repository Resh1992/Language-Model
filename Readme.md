## Language Model

We intend to implement language models. Use appropriate smoothing (you can use in built smoothing functions) to ensure your language model outputs a non-zero and valid probability distribution for out-of-vocabulary words as well. 

A dataset of movies reviews (positive and negative) is made available 

The program generates the following information:

1. The number of word tokens in the database.
2. Vocabulary size (number of unique words) of the dataset. 
3. Top ten bigrams and trigrams from positive and negative review sets, including the frequencies. 
4. Write a function, that given a sequence of three words (w1,w2,w3), would compute the probability of third word using trigram language model p(w3|w1,w2). If you're using log-probabilities, use base 2 for computing logs. 
5. Five test cases (sequence of three words) showing output from your trigram language model.

## Pre processing
Replaced few words like &lt;br&gt;, &lt;br /&gt; and &lt;br/&gt; with \n.<br />
We used regex to tokenize sentence into words. Regex used: [A-Z]{2,}(?![a-z])|[A-Z][a-z]+(?=[A-Z])|[\'\w\-]+<br />
Removed stop words.

## To run
python vocabulary-compute.py &lt;path-to-directory-containing-data&gt; 

