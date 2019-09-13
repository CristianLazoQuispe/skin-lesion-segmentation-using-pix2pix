# skin lesion segmentation using pix2pix

Se toma como referencia el trabajo:
## gan-skin-lesion
### [paper](https://arxiv.org/abs/1902.03253) "Skin Lesion Synthesis with Generative Adversarial Networks" in ISIC Skin Image Analysis Workshop and Challenge @ MICCAI 2018.
Disponible [here](https://github.com/alceubissoto/gan-skin-lesion)

Donde utilizan el dataset de 2018 ISIC Challenge teniendo como entrada una mascara semantica y como salida una imagen lesion cutanea.




### Results on CIFAR10
Note that in this repo, only the unsupervised version was implemented for now. I reaplced the orginal architecture with DCGAN and the results are more colorful than the original one.

From 0 to 100 epochs:

![cifar10](results/cifar10/cifar10.gif)



## Prerequisites
- Python 2.7
- PyTorch v0.2.0
- Numpy
- SciPy
- Matplotlib


## Getting Started
### Installation
- Install
