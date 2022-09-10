# AWD-LSTM
ROLE: 

University project for the course "Natural Language Processing" taught by Giuseppe Riccardi. It was a solo project with the goal to successfully pass the given baseline test perplexity with any combination of model and regularization technique. 

PROBLEM: 

Language modelling is the task of predicting the next word or character in a given document. It can be used to train language models that can further be applied to a wide range of natural language tasks, such as text generation, text classification, and question answering.
For this project we had to use the Penn Treebank dataset (word level).

SOLUTION: 

As the base model and the regularization techniques implemented were free-of-choice, I ended up using a simple stacked LSTM model and utilized several techniques from the AWD-LSTM paper | https://openreview.net/forum?id=SyyGPP0TZ.

Implemented regularization techniques:
- Weight dropout: randomly dropping weights rather than activations | https://paperswithcode.com/method/dropconnect
- Embedding dropout: randomly dropping embedded word representations | https://paperswithcode.com/method/embedding-dropout
- Weight tying: reduce number of parameters by sharing weights between the embedding and final activation layer | https://paperswithcode.com/method/weight-tying
- NT-ASGD: optimizer combining averaged and normal stochastic gradient descent | https://paperswithcode.com/method/nt-asgd

IMPACT: 

The project was successful as I managed to pass the given baseline test perplexity with over 22% (final result 70.66 after 100 epochs), which gave me the maximum grade and a possible thesis/internship offer in Giuseppe Riccardi's lab | http://sisl.disi.unitn.it/
