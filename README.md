# automl
Collection of resources on Machines programming Machines 


# 2017

## Neural Architecture Search

Neural networks are powerful and flexible models that work well for many difficult learning tasks in image, speech and natural language understanding. Despite their success, neural networks are still hard to design. In this paper, we use a recurrent network to generate the model descriptions of neural networks and train this RNN with reinforcement learning to maximize the expected accuracy of the generated architectures on a validation set. On the CIFAR-10 dataset, our method, starting from scratch, can design a novel network architecture that rivals the best human-invented architecture in terms of test set accuracy. Our CIFAR-10 model achieves a test error rate of 3.65, which is 0.09 percent better and 1.05x faster than the previous state-of-the-art model that used a similar architectural scheme. On the Penn Treebank dataset, our model can compose a novel recurrent cell that outperforms the widely-used LSTM cell, and other state-of-the-art baselines. Our cell achieves a test set perplexity of 62.4 on the Penn Treebank, which is 3.6 perplexity better than the previous state-of-the-art model. The cell can also be transferred to the character language modeling task on PTB and achieves a state-of-the-art perplexity of 1.214.

### Comments
Generates a string representing a model description. Train an RL algorithm using REINFORCE as learning strategy to optimize the hyperparameters of the RNN. Finds very good results on CIFAR10.

### Resources
[Paper](https://arxiv.org/pdf/1611.01578)
[Video](https://www.youtube.com/watch?v=XDtFXBYpl1w)
[Slides](http://rll.berkeley.edu/deeprlcoursesp17/docs/quoc_barret.pdf)
