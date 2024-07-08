# Anime Faces with DCGAN
Pictures generated by DCGAN: 

<img src="assets/output.png" alt="Anime DCGAN Output" />
 
Dataset-source is: <a href='https://www.kaggle.com/datasets/prasoonkottarathil/gananime-lite'> *here* </a>

A notebook related to this project also was published on the Kaggle: *here*

## Introducing
This project is the realization of the DCGAN model on the Keras. The main goal is to generate anime faces with a resolution of 128x128 px. The higher resolution requires more time and resources to train the model. 

## Generator architecture


<img src="assets/generator.png" alt="generator" />

## Discriminator architecture


<img src="assets/discriminator.png" alt="discriminator" />

## Training tips
Training process decsribed here: <a href='Anime Faces with DCGAN.ipynb'> *click* </a>

- For local training, I use Nvidia RTX 4050. (~12h of training 215 epochs).
 - Experiment with different train sizes for the discriminator and generator it will help you to stabilize the training. The best parameters are 0.00005 for the discriminator and 0.0002 for the generator. 
- Use gradient clipping to avoid exploding gradient
- You can replace BatchNormalization and Ralu layers with SELU for better training stabilization. (It increases the time of training by 6 hours) 

## Contributing 🙌
If you want to contribute to the project, your help is very welcome. This is an open-source project.

![](https://user-images.githubusercontent.com/45157446/161337980-87a1b2e4-99ea-4fc8-ab1e-faa61357b40d.gif)


 

## Acknowledgements 
This project was made possible thanks to:
- Different GAN Types described here: https://www.kaggle.com/code/rezasemyari/anime-gan-by-pytorch

- Siraj's Raval PokeGan https://www.kaggle.com/code/rezasemyari/anime-gan-by-pytorch

- The choice of learning rate by Alexia Jolicoeur-Martineau https://ajolicoeur.wordpress.com/cats/
