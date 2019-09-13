# Skin attribute detection using Generative Adversarial Networks-Pix2pix

En el presente trabajo se realiza la tarea de segmentacion semantica de lesiones cutaneas usando una red generativa adversaria (Generative Adversarial Networks) llamada Pix2pix.

## Se realiza dos pruebas:
### Ejemplo dataset para detección de atributos:
<ul>
  <li>pigment network</li>
  <li>negative network</li>
  <li>streaks</li>
  <li>milia-like cysts</li>
  <li> globules (including dots)</li>
</ul>
<img src="images/MAP_ISIC_0000013.jpg?raw=true" width="2500" height = "300"/>

### Ejemplo dataset para segmentacion de melanoma: 
<img src="images/SEGMENTATION_ISIC_0000013.jpg?raw=true" width="600" height = "200"/>



## Resultados

### Ejemplo dataset para detección de atributos:

<img src="images/ISIC_0013664.jpg?raw=true" height = "300"/><img src="images/ISIC_0013664.jpg?raw=true" height = "300"/> ![cifar10](images/OUTPUT_MAP.gif)



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
