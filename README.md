# Variational Neural Networks: Pytorch + Jax

This repository contains Pytorch and Jax implementations of Variational Neural Networks (VNNs) and image classification / uncertainty quality estimation experiments for [Variational Neural Networks paper](https://arxiv.org/abs/2207.01524).

Bayesian Neural Networks (BNNs) provide a tool to estimate the uncertainty of a neural network by considering a distribution over weights and sampling different models for each input. In this paper, we propose a method for uncertainty estimation in neural networks called Variational Neural Network that, instead of considering a distribution over weights, generates parameters for the output distribution of a layer by transforming its inputs with learnable sub-layers. In uncertainty quality estimation experiments, we show that VNNs achieve better uncertainty quality than Monte Carlo Dropout or Bayes By Backpropagation methods.

## Run
Use `pytorch/run_example.sh` to train and evaluate a single model on MNIST and `jax/run_example.sh` to train and evaluate a single model's uncertainty quality. Each script should be launched from the corresponding folder.

## Citation

If you use this work for your research, you can cite it as:
```
@article{oleksiienko2022vnn,
  author = {Oleksiienko, Illia and Tran, Dat Thanh and Iosifidis, Alexandros},
  journal={arxiv:2207.01524}, 
  title={Variational Neural Networks}, 
  year={2022},
}
```
