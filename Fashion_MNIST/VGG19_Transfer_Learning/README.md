## VGG19 [{Architecture}](https://iq.opengenus.org/vgg19-architecture/)
--------

In this model I used transfer learning approach and used the pretrained weights [whch were already trained on ImageNet Dataset] and added  a 10 class softmax layer at the end so as to classify the images into 10 classes. 
Only the weights of the last layer were trained and any experimentation with those considered for hyperparameter tuning

Details about hyperparameter tuning are given in the [.docx](https://github.com/Ayush8120/Image-Classification-DL/blob/main/Fashion_MNIST/VGG19_Transfer_Learning/HyperparameterTuning.docx) file 

Dataset Chosen : Fashion_MNIST
------------

As this dataset is GrayScale and VGG19 only takes RGB format of images as input thus we had to apply an extra step of preprocessing. Details about evry step written in the [.pynb](https://github.com/Ayush8120/Image-Classification-DL/blob/main/Fashion_MNIST/VGG19_Transfer_Learning/VGG19_Fashion_MNIST.ipynb) file

Model Metrics after 1 epoch
---------
    -Train Accuracy :  < 65%         
    -Validation Accuracy : 72.5%

Hyperparameters focussed upon :
------
    -Batch Size 
    -Type of optimizer  
    -Architecture of the introduced layers

Final Model with hyperparameters tuned
-------

    -Train Accuracy : 82. 98 %
    -Validation Accuracy : 81.81 %
    -Test Accuracy :  82.09 %

_Overfitting was strictly avoided and  the results obtained were_ : 
-----

<p align="center">
  <img width="400" height="400" src="https://lh6.googleusercontent.com/XibWWx4Rn5yQJVX4YrZRWfHAwyIVDsiOSzVpDp_3IT4lx3BwVxJH_JrtgCtgkLvy4c69uaJRAUU0GcagPyrD-E27suSpHWaRgTIpJj-uZpKqFXreXEIeRFquF390hfs-nR9aBfe9">
</p>

<p align="center">
  <img width="400" height="400" src="https://lh4.googleusercontent.com/n45od5po-nU90UKJgrU8uFeOPagAAhDOjEqZAdttr_ibAByDkTtsr0DWQyCccU_vMceZWbtvKS1aszrDbxpIxyuv8R8OPaMODE9BwUygGYstyXlVIkkgzKQtj5r3SM0S9BjKvX7j">
</p>

