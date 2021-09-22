### CNN Architecture For Image Classification On Fashion_MNIST dataset
I tried to implement image classification on Fashion MNIST Dataset using a fixed CNN Architecture. Main aim of the project was to understand how vastly the results vary when hyperparameter tuning is done properly.


#### Dataset Explaination :

**

<u>**<mark>Fashion MNIST Dataset:</mark>**</u>

Fashion-MNIST is a dataset of [Zalando](https://jobs.zalando.com/tech/)'s article images—consisting of a training set of 60,000 examples and a test set of 10,000 examples. Each example is a 28x28 grayscale image, associated with a label from 10 classes. We intend Fashion-MNIST to serve as a direct drop-in replacement for the original [MNIST dataset](http://yann.lecun.com/exdb/mnist/) for benchmarking machine learning algorithms. It shares the same image size and structure of training and testing splits.

Dataset links to understand and download:

- [A MNIST-like fashion product database. Benchmark](https://github.com/zalandoresearch/fashion-mnist)

- [Fashion MNIST](https://www.kaggle.com/zalando-research/fashionmnist)

- [fashion_mnist](https://www.tensorflow.org/datasets/catalog/fashion_mnist)

**

> +Train: Validation : Test dataset split taken as 40: 20: 10
> 
> +Data Augmentation was used to diversify the dataset
> 
> +Tried to optimise the performance solely on hyperparameter tuning 
> 
>     -moved ahead with the <u>constraint of fixed architecture</u> thus 
> 
>     -no change in number of filters and depth of network allowed

#### <u>Architecture Used</u>

**<img title="" src="https://lh5.googleusercontent.com/a4DrtcFLtq8YfZ-fnl8lHaVze2_ao-XzYKUNt8oIlKOG_QeszKGmtq56rb2XMMewCYvBJy5qJAp-JrO-fszflECzLVqBVlhU_sY8e7xORJPoBcor6aBI79e-1eQzfegYEDVEtLDP" alt="" width="286" data-align="inline">** 

**<img title="" src="https://lh5.googleusercontent.com/y0bW3vSiFi9d3jVPFbVK0ViMPXxY9SGV6t0iIz_JoJwSLDmvnFO88qdwydozv5hVA3v806gYzTSbwoZS--5kcXsK6Y6doZAncSXFP-kfMOY1mcbfGZe5G55xIVjFlH6neQ7OG2Hd" alt="" width="289" data-align="inline">**



##### <u>Training Accuracy and Validation Accuracy vs Epoch Count</u>

**![](https://lh6.googleusercontent.com/IB-sjTHUSV3Qwf9OLdG0j9g7IdlxyxXqLSRKDCPUMwV-HOuWg76z-Z8sp5J7XNGN5D-zbZpMxruMtWuaHEfPNNUvKC0jbIoXU5GyzgX0kATLAhIPsruc1KUfUZjyVfJz9UDsSHlz)**

##### <u>Training Loss and Validation Loss vs Epoch Count</u>



**![](https://lh5.googleusercontent.com/uj4ae0kxg3V1eHQW3KvgDA0Sfa8AZ7EIQa5PP0szc5dQrGe5wUUHo9qBF_shZrg3dTKszFclgUk7mXJ6vGhwAEi6XyuNaJxWMwJqYJrniMPh-fpqrCo2R7HlJiKasnXKS8Eg-JE0)**

> <mark>**Maximum Validation Accuracy Achieved**</mark> : 89.4%
> 
> <mark>**Training Accuracy at this Epoch**</mark> : 90.71%
> 
> <mark>**Test Accuracy achieved**</mark>: 91.17%
> 
> <mark>**Test Loss achieved**</mark>: 0.269255


