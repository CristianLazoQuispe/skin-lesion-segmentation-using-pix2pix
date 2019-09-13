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

### Ejemplo dataset para segmentacion de lesion: 
<img src="images/SEGMENTATION_ISIC_0000013.jpg?raw=true" width="600" height = "200"/>


## Preparing the data and environment
Para preparar todo automaticamente usar el bash `sh preparar.sh`
### Descargar el dataset
<ul>
  <li>ISIC2018_Task1-2_Training_Input</li>
  <li>ISIC2018_Task1_Training_GroundTruth</li>
  <li>ISIC2018_Task2_Training_GroundTruth_v3</li>
</ul>
Necesitamos descargar estos archivos del concurso [2018 ISIC Challenge](https://challenge2018.isic-archive.com/participate/) de la parte de training. Guardar las 3 carpetas en una carpeta "datasets"

### Configuring the enviroment.

Yo uso conda enviroments:
`conda create -n gansp3 python=3.7`
`conda activate gansp3`

### Install dependencies




## Resultados

### Ejemplo dataset para detección de atributos:
Para 50 epocas  para la imagen ISIC_0013664.jpg: 
####  Entrada_____________________________Original_____________________________Pix2pix
<img src="images/ISIC_0013664.jpg?raw=true" height = "256"/>  <img src="images/ISIC_0013664_map.jpg?raw=true" height = "256"/> ![cifar10](images/OUTPUT_MAP.gif)

<img src="images/MAP_test.jpg?raw=true" height = "256"/>


### Ejemplo dataset para segmentacion de lesion:
Para 50 epocas  para la imagen ISIC_0013664.jpg: 
####  Entrada_____________________________Original_____________________________Pix2pix
<img src="images/ISIC_0013664.jpg?raw=true" height = "256"/>  <img src="images/ISIC_0013664_map.jpg?raw=true" height = "256"/> ![cifar10](images/OUTPUT_MAP.gif)

<img src="images/MAP_test.jpg?raw=true"  height = "256"/>


# Referencias
Se toma como referencia el trabajo:
[paper](https://arxiv.org/abs/1902.03253) "Skin Lesion Synthesis with Generative Adversarial Networks" in ISIC Skin Image Analysis Workshop and Challenge @ MICCAI 2018. Donde utilizan el dataset de 2018 ISIC Challenge teniendo como entrada una mascara semantica y como salida una imagen de una lesion cutanea. Disponible [here](https://github.com/alceubissoto/gan-skin-lesion)

Se toma como referencia el trabajo:
[paper](https://arxiv.org/abs/1907.00856) "MobileGAN: Skin Lesion Segmentation Using a Lightweight Generative Adversarial Network" 


