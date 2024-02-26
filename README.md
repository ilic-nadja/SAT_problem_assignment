## CS6405 Datamining 

The assignment instructions are the following:

### Objective

The Boolean satisfiability (SAT) problem consists in determining whether a Boolean formula F is satisfiable or not. F is represented by a pair (X, C), where X is a set of Boolean variables and C is a set of clauses in Conjunctive Normal Form (CNF). Each clause is a disjunction of literals (a variable or its negation). This problem is one of the most widely studied combinatorial problems in computer science. It is the classic NP-complete problem. Over the past number of decades, a significant amount of research work has focused on solving SAT problems with both complete and incomplete solvers.

One of the most successful approaches is an algorithm portfolio, where a solver is selected among a set of candidates depending on the problem type. Your task is to create a classifier that takes as input the SAT instance's features and identifies the class.

In this project, we represent SAT problems with a vector of 327 features with general information about the problem, e.g., number of variables, number of clauses, the fraction of horn clauses in the problem, etc. There is no need to understand the features to be able to complete the assignment.

The original dataset is available at:

https://raw.githubusercontent.com/andvise/DataAnalyticsDatasets/main/train_dataset.cs v

Use the following template:

https://colab.research.google.com/drive/1_AX2wTRe6RoCX36HvP0UKSb13X3Gr77W?usp =sharing

### Tasks

Basic models and evaluation (5 Marks)

Using Scikit-learn, train a decision tree classifier using 70% of the dataset from training and 30% for testing. For this part of the project, we are not interested in optimising the parameters; we just want to get an idea of the dataset.

Robust evaluation (10 Marks)

In this section, we are interested in more rigorous techniques by implementing more sophisticated methods, for instance: ● Hold-out and cross-validation.

● Hyper-parameter tuning.

● Feature reduction.

● Feature normalisation.

Your report should provide concrete information about your reasoning; everything should be well-explained.

The key to getting good marks is to show that you evaluated different methods and that you correctly selected the configuration.

New classifier (10 Marks)

Replicate the previous task for a classifier that we did not cover in class. So different from K-NN and decision trees. Briefly describe your choice.

Try to create the best model for the given dataset.

Save your best model into your GitHub. And create a single code cell that loads it and evaluates it on the following test dataset:

https://github.com/andvise/DataAnalyticsDatasets/blob/main/test_dataset.csv

This link currently contains a sample of the training set. The real test set will be released after the submission. I should be able to run the code cell independently and load all the libraries you need as well.
