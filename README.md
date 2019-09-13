# Skin lesion segmentation using Generative Adversarial Networks-Pix2pix

En el presente trabajo se realiza la tarea de segmentacion semantica de lesiones cutaneas usando una red generativa adversaria (Generative Adversarial Networks) llamada Pix2pix.

## Se realiza dos pruebas:
### Ejemplo para map completo 
<img src="images/MAP_ISIC_0000013.jpg?raw=true" width="825" height = "200"/>

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


Se toma como referencia el trabajo:
[paper](https://arxiv.org/abs/1902.03253) "Skin Lesion Synthesis with Generative Adversarial Networks" in ISIC Skin Image Analysis Workshop and Challenge @ MICCAI 2018. Donde utilizan el dataset de 2018 ISIC Challenge teniendo como entrada una mascara semantica y como salida una imagen de una lesion cutanea. Disponible [here](https://github.com/alceubissoto/gan-skin-lesion)
