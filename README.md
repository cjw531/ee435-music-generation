# ee435-music-generation
## Disco Music Generation with VAEs
Reference: https://www.kaggle.com/basu369victor/generate-music-with-variational-autoencoder <br>
Dataset: https://www.kaggle.com/andradaolteanu/gtzan-dataset-music-genre-classification

We applied Variational Autoencoders (VAEs) to generate a music of a specific genre, a disco. It is based on Vector Quantized (VQ) VAE and a “Jukebox” model. Since VAEs are known to be generating noise or degrating the quality of the output, we increase sampling rate to discretize the music with higher fidelity, and change dimensionality of architecture accordingly. You may refer to the [`music_generation.ipynb`](https://github.com/cjw531/ee435-music-generation/blob/master/music_generation.ipynb) to see the final output of our generated music.

This work was done for the course <em>EE435: Deep Learning Foundations from Scratch</em> of [Northwestern Univeristy](https://www.northwestern.edu/).

## Project Video on YouTube
[![Music Generation with Variational Autoencoders (VAEs)](http://img.youtube.com/vi/3c3QWdrOH54/0.jpg)](https://www.youtube.com/watch?v=3c3QWdrOH54 "Music Generation with Variational Autoencoders (VAEs)")

## Environment Setup
In [conda](https://docs.conda.io/en/latest/) or [miniconda](https://docs.conda.io/en/latest/miniconda.html) environment, create a new environment for this repository, and activate it.<br>
Run the following command in your terminal to install the libraries:
```
pip install -r requirements.txt
```
Refer to the [`requirements.txt`](https://github.com/cjw531/ee435-music-generation/blob/master/requirements.txt) to see the full list of necessary libraries.

The code was tested in [Jupyter Notebook](https://jupyter.org/) and [Google Colab](https://colab.research.google.com/).

## Directory Structure
```bash
├── data/ ...contains the input disco music data
│   └── disco/
│       └── *.wav
├── plot/ ...contains the wave plot of generated music
│   ├── *.png ...per epoch
│   └── *.gif ...merged the epoch (static imgs) into animated file
├── img ...contains screenshots from rviz and rqt
│   └── /*.png
├── .gitignore
├── README.md
├── music_generation.ipynb ...implementation code
└── requirements.txt ...necessary libraries are listed
```
