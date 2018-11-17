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


# 2018

## Efficient Neural Architecture Search

We propose Efficient Neural Architecture Search (ENAS), a fast and inexpensive approach for automatic model design. In ENAS, a controller learns to discover neural network architectures by searching for an optimal subgraph within a large computational graph. The controller is trained with policy gradient to select a subgraph that maximizes the expected reward on the validation set. Meanwhile the model corresponding to the selected subgraph is trained to minimize a canonical cross entropy loss. Thanks to parameter sharing between child models, ENAS is fast: it delivers strong empirical performances using much fewer GPU-hours than all existing automatic model design approaches, and notably, 1000x less expensive than standard Neural Architecture Search. On the Penn Treebank dataset, ENAS discovers a novel architecture that achieves a test perplexity of 55.8, establishing a new state-of-the-art among all methods without post-training processing. On the CIFAR-10 dataset, ENAS designs novel architectures that achieve a test error of 2.89%, which is on par with NASNet (Zoph et al., 2018), whose test error is 2.65%.

### Comments
- 1000x less expensive than standard Neural Architecture Search
- Uses parameter sharing to improve the speed of architecture search
- Employs various training tricks to have a stable learning

### Resources
[Paper](https://arxiv.org/abs/1802.03268)
[Code](https://github.com/melodyguan/enas)
