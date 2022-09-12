# Finding Exoplanets with Astronomical Observations

Jason Terry

Google Summer of Code 2022

ML4Sci

<h1 align="center">
  <a href="https://www.python.org/"><img alt="Python" src="https://img.shields.io/badge/-Python 3.7+-blue?style=for-the-badge&logo=python&logoColor=white"></a>
  <a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/-PyTorch 1.8+-ee4c2c?style=for-the-badge&logo=pytorch&logoColor=white"></a>
  <a href="https://pytorchlightning.ai/"><img alt="Lightning" src="https://img.shields.io/badge/-Lightning 1.5+-792ee5?style=for-the-badge&logo=pytorchlightning&logoColor=white"></a>
  <a href="https://drive.google.com/file/d/1BBvAEeTYt2YJq9rdQlGEsI6YQ7pZqJI0/view?usp=sharing"><img alt="Explore in Google Colab" src="https://colab.research.google.com/assets/colab-badge.svg"></a>
  <a href="https://huggingface.co/spaces/chlab/interactive_kinematic_planet_detector"><img alt="Interact with Hugging Face" src="https://img.shields.io/badge/Interact%20-HuggingFace-f0cc4c.svg?style=for-the-badge&labelColor=gray"></a>
</h1>

This project is intended to use kinematic data of protoplanetary disks to determine whether a given observation has a planet and, if so, locate the planet or planets.

This repo includes two trained models and a small subset of both simulated and observational data that can be tested on. Run_97048 is raw data of disk HD 97048 taken from [DSHARP](https://almascience.eso.org/almadata/lp/DSHARP/).

The two architectures used are described below.

- RegNet
  - [Paper](https://arxiv.org/abs/2101.00590)
  - [Model Code](https://github.com/pytorch/vision/blob/main/torchvision/models/regnet.py)
  - [WANDB](https://wandb.ai/chlab/All_Coarse_Channels_regnet/sweeps/amna3jsu/overview?workspace=user-jpterry)
- EfficientNetV2
  - [Paper](https://arxiv.org/abs/2104.00298)
  - [Model Code](https://github.com/pytorch/vision/blob/main/torchvision/models/efficientnet.py)
  - [WANDB](https://wandb.ai/chlab/All_Coarse_Channels_efficientnet_v2_s/sweeps/q9fp4awl/overview?workspace=user-jpterry)

Hyperparameter sweeps using wandb were be done.

