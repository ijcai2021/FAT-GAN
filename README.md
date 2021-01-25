# FAT-GAN

**This is the implementation of Feature-Augmented and Transformed Generative Adversarial Network (FAT-GAN).**

## Introduction
Feature-Augmented and Transformed GAN (FAT-GAN) is implemented as an event generator that simulates particle production in electron-proton scattering that is free of theoretical assumptions about underlying particle dynamics. The difficulty of efficiently training a GAN event simulator lies in learning the complicated patterns of the distributions of the particles physical properties. We develop a GAN that selects a set of transformed features from particle momenta that can be generated easily by the generator, and uses these to produce a set of augmented features that improve the sensitivity of the discriminator. FAT-GAN is designed to faithfully reproduce the distribution of final state electron momenta in inclusive electron scattering, without the need for input derived from domain-based theoretical assumptions.

## Requirements
The code is written in Python3 and requires the following libraries:
* tensorflow==1.11.0
* keras==2.1.2

## Getting started
* Install the python libraries. (See [Requirements](https://github.com/ijcai2021/FAT-GAN#requirements)).
* Download the code from GitHub:
```bash
git clone https://github.com/ijcai2021/FAT-GAN
cd FAT-GAN
```

* Run the python script:
``` bash
python3 FAT-GAN.py
```
The script will read pythia data located in 'data/' and run for 200k epochs.

 ## Results:
 * Every 10k epochs, it will generate and save plots in 'gallery/'.
 
 
 [README](https://github.com/ijcai2021/FAT-GAN/README.md)
