Your Name : AN YOUNG PILL (Epsilon)

Your Email address : kokomong1316@gmail.com

1. Training Set Construction (5 pts)
Construct the training set for the amazon review dataset as instructed and report the following statistics.
Statistics


the total number of unique words in T


the total number of training examples in T


the ratio of positive examples to negative examples in T


the average length of document in T


the max length of document in T



2. Performance of deep neural network for classification (20 pts)

Suggested hyperparameters: 
	
Data processing: 
Word embedding dimension: 100
Word Index: keep the most frequent 10k words
CNN
Network: Word embedding lookup layer -> 1D CNN layer -> fully connected layer -> output prediction
Number of filters: 100
Filter length: 3
CNN Activation: Relu
Fully connected layer dimension 100, activation: None (i.e. this layer is linear)
RNN:
Network: Word embedding lookup layer -> LSTM layer -> fully connected layer(on the hidden state of the last LSTM cell) -> output prediction
Hidden dimension for LSTM cell: 100
Activation for LSTM cell: tanh
Fully connected layer dimension 100, activation: None (i.e. this layer is linear)
	


Accuracy
Training time(in seconds)
RNN w/o pretrained embedding




RNN w/ pretrained embedding




CNN w/o pretrained embedding




CNN w/ pretrained embedding







3. Training behavior (10 pts)


Plot the training/testing objective, training/testing accuracy over time for the 4 model combinations (correspond to 4 rows in the above table). In other word, there should be 2*4=8 graphs in total, each of which contains two curves (training and testing).
RNN w/o pretrained embedding
training/testing objective over time
training/testing accuracy over time
RNN w/ pretrained embedding
training/testing objective over time
training/testing accuracy over time
CNN w/o pretrained embedding
training/testing objective over time
training/testing accuracy over time
CNN w/ pretrained embedding
training/testing objective over time
training/testing accuracy over time

4. Analysis of results (10 pts)


Discuss the complete set of experimental results, comparing the algorithms to each other. Discuss your observations about the various algorithms, i.e., differences in how they performed, different parameters, what worked well and didn't, patterns/trends you observed across the set of experiments, etc.  Try to explain why certain algorithms or approaches behaved the way they did.








5. The software implementation (5 pts)
Add detailed descriptions about software implementation & data preprocessing, including:
   1. A description of what you did to preprocess the dataset to make your implementations easier or more efficient.





   2. A description of major data structures (if any); any programming tools or libraries that you used;






   3. Strengths and weaknesses of your design, and any problems that your system encountered;
