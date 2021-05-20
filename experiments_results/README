# Appendix A: Log files for a set of experiments

## Description

Each file in this folder contains the results of an elementary CBOW classifier using a particular embedding model on a particular dataset.
The file names are constructed as such: `<Embedding>_<Dataset>.log`.

## Log Files

Each log files contains (in order):

- The configuration of the experiment, after automatic fine-tuning, listing in particular: the embedding model and corpus, the batch size, the hyper-parameters of the Adam optimizer (beta1, beta2, lr), the reduction factor (gamma) of the learning rate decay scheduler on validation metric plateaus, and the number of epochs.

- The test set evaluation results, followed by the associated report, as well as the equivalent report for the Dummy (random stratified) baseline classifier.

- The analysis of the weights of the classifier: for each class label (formatted: `- <label> [precision = <precision for this class>] :`), we list the top-10 positive predicting dimensions (highest discriminating weights) and top-10 negative predicting dimensions (lowest discriminating weights) with the following formatting:
`-- <dimension number> {<weight>} [<for dual input datasets: position of the weight in the composition vector (first/second vector, element-wise product, or absolute difference)>] : <list of top-10 most active words for this dimension in the embedding model>`
