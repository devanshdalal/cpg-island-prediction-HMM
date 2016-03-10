Input and Output Files Format:

Sequence Files: "training.txt" is the input genomic sequence. The whole sequence
is divided in multiple lines and such format is known as multi-fasta.  Note that
the length of the complete sequence for the given training file should be 85000.
A similar test file (testing.txt) is given to you.

FILE cpg_island_training.txt format: You are given a separate file 
denoting the cpg islands in the training sequence where:
1. Each line of this file denotes a cpg island in the above sequence.  
2. Consider the following.  347 584. It denotes that the cpg island starts
from position 347 and ends at position 584 (584 included).  

You need to generate a similar cpg_island file for the test data using
your learned model. For your reference, we are also providing
the true locations of the cpg islands in the given test sequence (see
file cpg_island_test.txt). You can compare the output (prediction) of 
your program with the annotation in this file to determine how well your
program does in comparison to the true annotation.

Your program should be able to do the following:

1. Given a training data file and the corresponding file denoting cpg
islands in the sequence, learn the HMM model.
2. Test your model on the given test sequence. The output should be the
file containing the predicated cpg islands in the test sequence in the format
specified above.

During the demo, we would also run your programs on completely new train/test
sequences (possibly of different lengths than in the provided dataset). 
Your program should be learn the desired model and output the cpg islands
in the test sequence. 
