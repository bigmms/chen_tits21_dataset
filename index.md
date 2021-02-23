---
layout: default
---

<img src="./figure/demo.png" width="640" height="480" align="middle" />

# News
* **2021-02-23** Amount of images of **glare image dataset** are all increased to 87.5k now.
* **2020-02-23** If Google Drive is not accessible, please download the dataset using Baidu Drive.

## Abstract
Using de-hazing, de-raining, and de-reflection methods to eliminate glare from a single image is challenging. In this study, we formulated sun glare removal as an image decomposition problem. We solved this problem by developing a single-image-based sun glare removal network, which can achieve accurate glare segmentation and removal with high quality visual perception. To enable end-to-end discriminative learning in our network, we synthesized multiple glare images according to the glare image formation model. In the synthesis procedure, we randomly set the sun rays to have diversified sizes, shapes, densities, and positions in the aforementioned model. To the best of our knowledge, this study is among the first to construct a large-scale sun glare image dataset comprising glare and glare-free image pairs of different license plates and the corresponding decomposed components of the images.

## Overview
**glare image dataset**, a large-scale dataset for synthesized sun glare, features three appealing properties: good quality, large scale, and high diversity. A total of **1,166** glare-free license plate images with different plate numbers were collected from ETC systems. The glare-free images in our dataset were divided into two subsets, namely the training and testing subsets. We randomly sampled **1,000** glare-free images to be the training set, and the remaining **166** glare-free images comprised the testing set. There are **75** base masks which could be classified into **6** subset to simulate the catoptric behaviors of sunlight. The number of synthesized glare images in each subset is presented in Details part.

## Details
We contribute **glare image dataset**, a large-scale sun glare image dataset, which has several appealing properties:
- All images in **glare image dataset** are normalized into a size of **80 * 176** pixels.

- **glare image dataset** consists of **87.5k** synthesized glare images, glare-free images, occlusion images, and foreground images.

- To simulate the catoptric behaviors of sunlight to synthesize glare images, each base masks could be classified into **6** subset:

| Subset          | Hexagonal | Octagonal | Star | Triangular | Rectangular | Ring |
|:----------------|:----------|:----------|:------------|:-----------|:------------|:------------|
| #base masks     |       12  | 15  |12|13|16|7|
| #training image |    12000  | 15000|12000|13000|16000|7000|
| #testing image  |     1922  | 2490|1992|2158|2656|1162|

## Space Requirement
* Training Set: ~2.4 GB
* Testing Set: ~500 MB
* Total: ~3 GB

## Data Structure
After unzipping the files, you will get all the data in the following folder structure:
```
dataset
|--test
   |--foreground_images
      <several foreground images>
   |--glare-free_images
      <several glare-free images>
   |--occlusion_images
      <several occlusion images>
   |--synthesized_glare_images
      <several synthesized glare images>
|--train
   |--foreground_images
      <several foreground images>
   |--glare-free_images
      <several glare-free images>
   |--occlusion_images
      <several occlusion images>
   |--synthesized_glare_images
      <several synthesized glare images>
```

## Sample Images
<img src="./figure/sample.png" width="640" height="300" align="middle" />

## Download

* Paper [[PDF]](https://ieeexplore.ieee.org/document/9357944)
* glare image dataset [[Google Drive]](https://drive.google.com/drive/folders/1He7MLn-7Kcvdj6rJPpF50xR0e21vqQ0R?usp=sharing) [[Baidu Drive]](https://pan.baidu.com/s/1I4I2ge8uJfSciB-VeB2imw) (password: bkf1)

## Agreement
* The **glare image dataset** is available for non-commercial research purposes only.
* You agree not to reproduce, duplicate, copy, sell, trade, resell or exploit for any commercial purposes, any portion of the images and any portion of derived data.
* You agree not to further copy, publish or distribute any portion of the **glare image dataset**. Except, for internal use at a single site within the same organization it is allowed to make copies of the dataset.
* The BigMMS Laboratory reserves the right to terminate your access to the **glare image dataset** at any time.

## Attribution
```
@ARTICLE{ChenTITS2021,
  author={B. -H. {Chen} and S. {Ye} and J. -L. {Yin} and H. -Y. {Cheng} and D. {Chen}},
  journal={IEEE Transactions on Intelligent Transportation Systems}, 
  title={Deep Trident Decomposition Network for Single License Plate Image Glare Removal}, 
  year={2021},
  volume={},
  number={},
  pages={1-12},
  doi={10.1109/TITS.2021.3058530}}
```

## Contact

Please contact [Hsiang-Yin Cheng](mailto:qwaszx841002@gmail.com), [Jia-Li Yin](mailto:jlyin@fzu.edu.cn), or [Bo-Hao Chen](mailto:bhchen@saturn.yzu.edu.tw) for questions about the dataset.
