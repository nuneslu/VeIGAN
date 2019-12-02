# VeIGAN: Vectorial Inpainting Generative Adversarial Networks for Depth Maps Object Removal

![VeIGAN GIF](https://github.com/nuneslu/VeIGAN/blob/master/examples/IVGif.gif)

## About
This code is based on the Generative Inpainting [CVPR 2018](https://arxiv.org/abs/1801.07892) paper and it's [repository](https://github.com/JiahuiYu/generative_inpainting).

Based on the Generative Inpainting network we proposed adaptations to deal with disparity images inpainting. Our results have been publish on [IV 2019](https://ieeexplore.ieee.org/document/8814157) and on this repository we have the code used on this publication.

## Installation

To use this code, please follow the installation instructions from the original repository since the dependencies are the same.

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
For the paper all the train and test were made in a GeForce GTX 1080ti.

## VeIGAN Examples

Depth map object removal example and the respective 3D mesh reconstruction:

![Disparity Inpainting](https://github.com/nuneslu/VeIGAN/blob/master/examples/example.png)
![CityScapes Disparity Inpainting](https://github.com/nuneslu/VeIGAN/blob/master/examples/spoiler_result.png)


## License

CC 4.0 Attribution-NonCommercial International

The software is for educaitonal and academic research purpose only.

## Citations

Please cite this work as follow:

@INPROCEEDINGS{8814157,\n
author={L. P. N. {Matias} and M. {Sons} and J. R. {Souza} and D. F. {Wolf} and C. {Stiller}},\n
booktitle={2019 IEEE Intelligent Vehicles Symposium (IV)},
title={VeIGAN: Vectorial Inpainting Generative Adversarial Network for Depth Maps Object Removal},
year={2019},
volume={},
number={},
pages={310-316},
doi={10.1109/IVS.2019.8814157},
ISSN={1931-0587},
month={June},}
