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

The different datasets in matlab format are located in these locations:

 - [emnist-letters.mat](https://github.com/sherpaai/federated-emnist-dataset/blob/master/datasets/emnist-letters.mat)
 - [emnist-digits.mat](https://github.com/sherpaai/federated-emnist-dataset/blob/master/datasets/emnist-digits.mat)
 - [eminst-mnist.mat](https://github.com/sherpaai/federated-emnist-dataset/blob/master/datasets/emnist-mnist.mat)


## How to use it

 - You can import them in your code using [scipy.io.loadmat function](https://docs.scipy.org/doc/scipy/reference/generated/scipy.io.loadmat.html). For example, for the EMNIST Letters dataset:
 
 ```python
    dataset = scipy.io.loadmat(./emnist-digits.mat)['dataset']
    train_images = dataset['train'][0,0]['images'][0,0]
    train_labels = dataset['train'][0,0]['labels'][0,0]
    test_images = dataset['test'][0,0]['images'][0,0]
    test_labels = dataset['test'][0,0]['labels'][0,0]
 ```

## References

The datasets in this repo are recollected from [NIST - The EMNIST Dataset](https://www.nist.gov/itl/products-and-services/emnist-dataset).
