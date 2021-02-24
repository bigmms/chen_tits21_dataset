---
layout: default
---

<img src="./figure/demo.png" width="640" height="480" align="middle" />

# News
* **2020-02-23** If Google Drive is not accessible, please download the dataset using Baidu Drive.

## Overview
**Sun glare image dataset**, a new dataset for synthesized sun glare, features three appealing properties: good quality, large scale, and high diversity. A total of **1,166** glare-free license plate images with different plate numbers were collected at road during morning commute traffic. The glare-free images in our dataset were divided into two subsets, namely the training and testing subsets. We randomly sampled **1,000** glare-free images to be the training set, and the remaining **166** glare-free images comprised the testing set. There are **75** base masks which could be classified into **6** subset to simulate the catoptric behaviors of sunlight. The number of synthesized glare images in each subset is presented in **Details** part.

## Details
We contribute **Sun glare image dataset**, a large-scale sun glare image dataset, which has several appealing properties:
- All images in **Sun glare image dataset** are normalized into a size of **80 * 176** pixels.

- **Sun glare image dataset** consists of **87.5k** synthesized glare images, glare-free images, occlusion images, and foreground images.

- To simulate the catoptric behaviors of sunlight to synthesize glare images, each base masks could be classified into **6** subset. See the table below.

| Subset          | Hexagonal | Octagonal | Star | Triangular | Rectangular | Ring |
|:----------------|----------:|----------:|------------:|-----------:|-----------:|-----------:|
| #base masks     |       12  | 15  |12|13|16|7|
| #training images |    12000  | 15000|12000|13000|16000|7000|
| #testing images  |     1922  | 2490|1992|2158|2656|1162|

## Space Requirement
* Training Set: ~2.4 GB
* Testing Set: ~500 MB
* Total: ~3 GB

## Data Structure
After unzipping the files, you will get all the data in the following folder structure:
```
dataset
|--train
   |--foreground_images
      <several foreground images>
   |--glare-free_images
      <several glare-free images>
   |--occlusion_images
      <several occlusion images>
   |--synthesized_glare_images
      <several synthesized glare images>
|--test
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
<img src="./figure/sample.png" width="640" height="448" align="middle" />

## Agreement
Before downloading and using the **Sun glare image dataset**, please agree to the following terms of use. You, your employer and your affiliations are referred to as “User”. The authors and their affiliations, Yuan Ze University, are referred to as “Producer”.

(1) The **Sun glare image dataset** is used for non-commercial/non-profit research purposes only.

(2) All the source images in **Sun glare image dataset** collected by the Producer are supported by the Ministry of Science and Technology, Taiwan under Grant MOST 108-2221-E-155-034-MY3 and Grant MOST 107-2221-E-155-052-MY2. All the images in **Sun glare image dataset** can be used for academic purposes. However, the Producer is NOT responsible for any further use in a defamatory, pornographic or any other unlawful manner, or violation of any applicable regulations or laws.

(3) The User takes full responsibility for any consequence caused by his/her use of **Sun glare image dataset** in any form and shall defend and indemnify the Producer against all claims arising from such uses.

(4) The User should NOT distribute, copy, reproduce, disclose, assign, sublicense, embed, host, transfer, sell, trade, or resell any portion of the **Sun glare image dataset** to any third party for any purpose.

(5) The User can provide his/her research associates and colleagues with access to **Sun glare image dataset** (the download link or the dataset itself) provided that he/she agrees to be bound by these terms of use and guarantees that his/her research associates and colleagues agree to be bound by these terms of use.

(6) The User should NOT remove or alter any copyright, trademark, or other proprietary notices appearing on or in copies of the **Sun glare image dataset**.

(7) This agreement is effective for any potential User of the **Sun glare image dataset** upon the date that the User first accesses the **Sun glare image dataset** in any form.

(8) The Producer reserves the right to terminate the User’s access to the **Sun glare image dataset** at any time.

(9) For using **sun glare image dataset**, please cite the following papers:
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
```
@INPROCEEDINGS{YeICIP20,
author={S. {Ye} and J. -L. {Yin} and B. -H. {Chen} and D. {Chen} and Y. {Wu}},
booktitle={IEEE International Conference on Image Processing (ICIP)},
title={Single Image Glare Removal Using Deep Convolutional Networks},
year={2020},
volume={},
number={},
pages={201-205},
doi={10.1109/ICIP40778.2020.9190712}}
```

## Download
* [[Google Drive]](https://drive.google.com/drive/folders/1He7MLn-7Kcvdj6rJPpF50xR0e21vqQ0R?usp=sharing) 
* [[Baidu Drive]](https://pan.baidu.com/s/1I4I2ge8uJfSciB-VeB2imw) (password: bkf1)

## Benchmark
We benchmark seven representative atmospheric obscuration removal methods using the **Sun glare image dataset**. Please refer to our [paper](https://ieeexplore.ieee.org/document/9357944) for more information.

## Contact
Please contact [Hsiang-Yin Cheng](mailto:qwaszx841002@gmail.com), [Jia-Li Yin](mailto:jlyin@fzu.edu.cn), or [Bo-Hao Chen](mailto:bhchen@saturn.yzu.edu.tw) for questions about the dataset.

<!-- 由 Google 結構化資料標記協助工具產生的 JSON-LD 標記。 -->
<script type="application/ld+json">
{
  "@context" : "http://schema.org",
  "@type" : "Dataset",
  "name" : "Sun Glare Image Dataset",
  "description" : "Sun glare image dataset, a new dataset for synthesized sun glare, features three appealing properties: good quality, large scale, and high diversity.",
  "version" : "1.0",
  "distribution" : {
    "@type" : "DataDownload",
    "contentUrl" : "https://bigmms.github.io/chen_tits21_dataset/"
  },
  "sourceOrganization" : "BigMMS Laboratory",
  "datePublished" : "2021-02-23"
}
</script>
