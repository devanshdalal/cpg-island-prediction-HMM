### Viterbi Algorithm

Devansh Dalal
Report of Assignment 2(b)
­­­­­
Note: All the code is mainly implemented in Python. 

## Finding CPGs islands in the sequence

Commands :  python 2b.py <path to the testing file>
Where path to the training data is assumed to be  ../gene_data/  .

Viterbi Algorithm:

To avoid overflows, I have used log of the probabilities instead of probabilities in the computations of probabilities of hidden states for each index i. And also no state cannot be assigned zero probability as log(0) is not defined so we assign a very small number () if probability is zero. In this approach the log-probability of the most likely sequence will be
 
For test data the log of probability of most likely state was found to be


## Time complexity: 

The transition, emission and initial probabilities are computed as mentioned in the assignment and Viterbi algorithm is implemented for calculating the most likely states of the hidden sequence.

where n is the length of the sequence and S is the set of all possible states. Since we have |S|=8 for all indexes of the sequence. Therefore final complexity will be.

## Connection between Max-product VE and Viterbi

The max-product VE and Viterbi both necessarily calculates the same result i.e. most-probable cumulative assignment of variables over the given Markov network. The max-product VE is more general as compared to the Viterbi algorithm applied here on the linear chain. But they calculates the same inference.


## References

1. http://www.cse.iitd.ac.in/~parags/teaching/col776/assignments/ass1-b/ass2-b.pdf

2. https://en.wikipedia.org/wiki/Viterbi_algorithm