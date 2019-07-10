# VeIGAN: Vectorial Inpainting Generative Adversarial Networks for Depth Maps Object Removal

## About
This code is based on the Generative Inpainting [CVPR 2018](https://arxiv.org/abs/1801.07892) paper and it's [repository](https://github.com/JiahuiYu/generative_inpainting).

Based on the Generative Inpainting network we proposed adaptations to deal with disparity images inpainting. Our results have been publish on the [IV 2019](https://iv2019.org/) and on this repository we have the code used on this publication.

## Installation

To use this code, please follow the installation instructions from the original repository since de dependencies are the same.

## Usage

The directory _/training_data_ has the disparity images for the training and the _/data_flist_ contains the _.flist_ files wich list the images.

For training the command is:
```
python3 train.py
```

For testing use:
```
python3 test.py --image 'input_image' --mask 'removed_area_mask' --output 'output_image' --checkpoint_dir model_logs/'trained_model_dir'
```

## Disparity Inpainting Examples

Object removal and 3D mesh reconstruction for comparison:
