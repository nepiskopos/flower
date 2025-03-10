# Flower: A Friendly Federated Learning Framework

<p align="center">
  <a href="https://flower.dev/">
    <img src="https://flower.dev/_next/image/?url=%2F_next%2Fstatic%2Fmedia%2Fflower_white_border.c2012e70.png&w=640&q=75" width="140px" alt="Flower Website" />
  </a>
</p>
<p align="center">
    <a href="https://flower.dev/">Website</a> |
    <a href="https://flower.dev/blog">Blog</a> |
    <a href="https://flower.dev/docs/">Docs</a> |
    <a href="https://flower.dev/conf/flower-summit-2022">Conference</a> |
    <a href="https://flower.dev/join-slack">Slack</a>
    <br /><br />
</p>

[![GitHub license](https://img.shields.io/github/license/adap/flower)](https://github.com/adap/flower/blob/main/LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/flower/blob/main/CONTRIBUTING.md)
![Build](https://github.com/adap/flower/actions/workflows/flower.yml/badge.svg)
![Downloads](https://pepy.tech/badge/flwr)
[![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://flower.dev/join-slack)

Flower (`flwr`) is a framework for building federated learning systems. The
design of Flower is based on a few guiding principles:

* **Customizable**: Federated learning systems vary wildly from one use case to
  another. Flower allows for a wide range of different configurations depending
  on the needs of each individual use case.

* **Extendable**: Flower originated from a research project at the University of
  Oxford, so it was built with AI research in mind. Many components can be
  extended and overridden to build new state-of-the-art systems.

* **Framework-agnostic**: Different machine learning frameworks have different
  strengths. Flower can be used with any machine learning framework, for
  example, [PyTorch](https://pytorch.org),
  [TensorFlow](https://tensorflow.org), [Hugging Face Transformers](https://huggingface.co/), [PyTorch Lightning](https://pytorchlightning.ai/), [MXNet](https://mxnet.apache.org/), [scikit-learn](https://scikit-learn.org/), [JAX](https://jax.readthedocs.io/), [TFLite](https://tensorflow.org/lite/), [fastai](https://www.fast.ai/), [Pandas](https://pandas.pydata.org/
) for federated analytics, or even raw [NumPy](https://numpy.org/)
  for users who enjoy computing gradients by hand.

* **Understandable**: Flower is written with maintainability in mind. The
  community is encouraged to both read and contribute to the codebase.

Meet the Flower community on [flower.dev](https://flower.dev)!

## Federated Learning Tutorial

Flower's goal is to make federated learning accessible to everyone. This series of tutorials introduces the fundamentals of federated learning and how to implement them in Flower.

1. **An Introduction to Federated Learning**

   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb))

2. **Using Strategies in Federated Learning**

   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb))
   
3. **Building Strategies for Federated Learning**

   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb))
   
4. **Custom Clients for Federated Learning**

   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb))

Stay tuned, more tutorials are coming soon. Topics include **Privacy and Security in Federated Learning**, and **Scaling Federated Learning**.

## Documentation

[Flower Docs](https://flower.dev/docs):
* [Installation](https://flower.dev/docs/installation.html)
* [Quickstart (TensorFlow)](https://flower.dev/docs/quickstart-tensorflow.html)
* [Quickstart (PyTorch)](https://flower.dev/docs/quickstart-pytorch.html)
* [Quickstart (Hugging Face [code example])](https://flower.dev/docs/quickstart-huggingface.html)
* [Quickstart (PyTorch Lightning [code example])](https://flower.dev/docs/quickstart-pytorch-lightning.html)
* [Quickstart (MXNet)](https://flower.dev/docs/example-mxnet-walk-through.html)
* [Quickstart (Pandas)](https://flower.dev/docs/quickstart-pandas.html)
* [Quickstart (fastai)](https://flower.dev/docs/quickstart-fastai.html)
* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)
* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)
* [Quickstart (TFLite on Android [code example])](https://github.com/adap/flower/tree/main/examples/android)

## Flower Baselines

Flower Baselines is a collection of community-contributed experiments that reproduce the experiments performed in popular federated learning publications. Researchers can build on Flower Baselines to quickly evaluate new ideas:

* [FedAvg](https://arxiv.org/abs/1602.05629):
  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedavg_mnist)
* [FedProx](https://arxiv.org/abs/1812.06127):
  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedprox_mnist)
* [FedBN: Federated Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/abs/2102.07623):
  * [Convergence Rate](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedbn/convergence_rate)
* [Adaptive Federated Optimization](https://arxiv.org/abs/2003.00295):
  * [CIFAR-10/100](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/adaptive_federated_optimization)

Check the Flower documentation to learn more: [Using Baselines](https://flower.dev/docs/using-baselines.html)

The Flower community loves contributions! Make your work more visible and enable others to build on it by contributing it as a baseline: [Contributing Baselines](https://flower.dev/docs/contributing-baselines.html)

## Flower Usage Examples

Several code examples show different usage scenarios of Flower (in combination with popular machine learning frameworks such as PyTorch or TensorFlow).

Quickstart examples:

* [Quickstart (TensorFlow)](https://github.com/adap/flower/tree/main/examples/quickstart_tensorflow)
* [Quickstart (PyTorch)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch)
* [Quickstart (Hugging Face)](https://github.com/adap/flower/tree/main/examples/quickstart_huggingface)
* [Quickstart (PyTorch Lightning)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch_lightning)
* [Quickstart (fastai)](https://github.com/adap/flower/tree/main/examples/quickstart_fastai)
* [Quickstart (Pandas)](https://github.com/adap/flower/tree/main/examples/quickstart_pandas)
* [Quickstart (MXNet)](https://github.com/adap/flower/tree/main/examples/quickstart_mxnet)
* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)
* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)
* [Quickstart (TFLite on Android)](https://github.com/adap/flower/tree/main/examples/android)

Other [examples](https://github.com/adap/flower/tree/main/examples):

* [Raspberry Pi & Nvidia Jetson Tutorial](https://github.com/adap/flower/tree/main/examples/embedded_devices)
* [Android & TFLite](https://github.com/adap/flower/tree/main/examples/android)
* [PyTorch: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/pytorch_from_centralized_to_federated)
* [MXNet: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/mxnet_from_centralized_to_federated)
* [Advanced Flower with TensorFlow/Keras](https://github.com/adap/flower/tree/main/examples/advanced_tensorflow)
* [Advanced Flower with PyTorch](https://github.com/adap/flower/tree/main/examples/advanced_pytorch)
* Single-Machine Simulation of Federated Learning Systems ([PyTorch](https://github.com/adap/flower/tree/main/examples/simulation_pytorch)) ([Tensorflow](https://github.com/adap/flower/tree/main/examples/simulation_tensorflow))

## Community

Flower is built by a wonderful community of researchers and engineers. [Join Slack](https://flower.dev/join-slack) to meet them, [contributions](#contributing-to-flower) are welcome.

<a href="https://github.com/adap/flower/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=adap/flower" />
</a>

## Citation

If you publish work that uses Flower, please cite Flower as follows: 

```bibtex
@article{beutel2020flower,
  title={Flower: A Friendly Federated Learning Research Framework},
  author={Beutel, Daniel J and Topal, Taner and Mathur, Akhil and Qiu, Xinchi and Parcollet, Titouan and Lane, Nicholas D},
  journal={arXiv preprint arXiv:2007.14390},
  year={2020}
}
```

Please also consider adding your publication to the list of Flower-based publications in the docs, just open a Pull Request.

## Contributing to Flower

We welcome contributions. Please see [CONTRIBUTING.md](CONTRIBUTING.md) to get started!
