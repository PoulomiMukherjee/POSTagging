# POS tagging using modified Viterbi

#### Problem Statement:

The vanilla Viterbi algorithm generally faces a high loss of accuracy majorly due to the fact that when the algorithm encounters an unknown word which was not present in the training set, it assigns an incorrect tag arbitrarily. This is because, for unknown words, the emission probabilities for all candidate tags are 0, so the algorithm arbitrarily chooses (the first) tag.

Using the Treebank dataset of NLTK with the 'universal' tagset, the Viterbi algorithm should be modified to solve the problem of unknown words using at least two techniques. The main objectives are:

- To write the vanilla Viterbi algorithm for assigning POS tags (i.e. without dealing with unknown words)
- To solve the problem of unknown words using at least two techniques. These techniques can use any of the approaches discussed in the class - lexicon, rule-based, probabilistic etc.
- To compare the tagging accuracy after making these modifications with the vanilla Viterbi algorithm.
- To list down at least three cases from the sample test file (i.e. unknown word-tag pairs) which were incorrectly tagged by the original Viterbi POS tagger and got corrected after your modifications.

#### Project Pipeline:

The steps that have been followed are mentioned below:

1. Build the vanilla Viterbi based POS tagger
2. Build Modified Viterbi I using probabilistic technique
3. Build Modified Viterbi II using rule-based backoff method
