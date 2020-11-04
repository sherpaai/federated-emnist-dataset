# The Extended EMNIST (EMNIST) Dataset

According to [NIST](https://www.nist.gov/itl/products-and-services/emnist-dataset), the EMNIST dataset is a set of 
handwritten character digits derived from the [NIST Special Database 10](https://www.nist.gov/srd/nist-special-database-19)
and converted to a 28x28 pixel image format and dataset structure that directly matches de [MNIST dataset](http://yann.lecun.com/exdb/mnist/).
For further information refer to the [EMNIST paper](https://arxiv.org/abs/1702.05373v1).

## Dataset summary

There are multiple splits provided in [NIST](https://www.nist.gov/itl/products-and-services/emnist-dataset). However,
for the moment we provided the following:

1. EMNIST Letters: 145,600 characters. 26 balanced classes.
2. EMNIST Digits: 280,000 characters. 10 balanced classes.
3. EMNIST MNIST: 70,000 characters. 10 balanced classes.

Please, check the [EMNIST paper](https://arxiv.org/abs/1702.05373v1) for further details about the dataset structure.

## Download datasets

The different datasets are located in these locations:

 - [emnist-letters.zip](https://github.com/sherpaai/federated-emnist-dataset/datasets/emnist-letters.zip)
 - [emnist-digits.zip](https://github.com/sherpaai/federated-emnist-dataset/datasets/emnist-digits.zip)
 - [eminst-mnist.zip](https://github.com/sherpaai/federated-emnist-dataset/datasets/emnist-mnist.zip)


## How to use it

 - You can import them in your code using [numpy.load function](https://numpy.org/doc/stable/reference/generated/numpy.load.html).
 For example, for EMNIST Digits dataset:
 
 ```python
    data = np.load('./emnist-digits.zip')
 ```

## Requirements

This work is tested with Python 3.8.5.

The requirements.txt file is automatically generated with [pipreqs](https://github.com/bndr/pipreqs).

## References

The datasets in this repo are recollected from [NIST - The EMNIST Dataset](https://www.nist.gov/itl/products-and-services/emnist-dataset).
