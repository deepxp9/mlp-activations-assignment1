# Assignment 1: Multilayer perceptron for images

The textbook MLP from *Generative Deep Learning* (2nd ed.), [`02_deeplearning/01_mlp/mlp.ipynb`](https://github.com/davidADSP/Generative_Deep_Learning_2nd_Edition/blob/main/notebooks/02_deeplearning/01_mlp/mlp.ipynb), trained on CIFAR-10 in three versions that differ only in the hidden-layer activation function:

1. ReLU
2. LeakyReLU
3. Sigmoid

**Notebook:** [mlp_activations_assignment1.ipynb](mlp_activations_assignment1.ipynb), including training, evaluation and the interpretation of the output and accuracy (section 5).

| Activation | Test accuracy | Test loss |
|---|---|---|
| ReLU | 48.6% | 1.454 |
| LeakyReLU | 48.1% | 1.462 |
| Sigmoid | 47.1% | 1.471 |

Setup (same as the textbook): Flatten -> Dense(200) -> Dense(150) -> Dense(10, softmax), Adam (lr 0.0005), batch size 32, 10 epochs.
