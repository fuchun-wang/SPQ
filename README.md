## Self-supervised Product Quantization for Deep Unsupervised Image Retrieval
Pytorch implementation of SPQ   
Accepted to ICCV 2021 - <a href="https://arxiv.org/pdf/2109.02244.pdf">paper</a>  
Young Kyun Jang and Nam Ik Cho  

## Abstract

Supervised deep learning-based hash and vector quantization are enabling fast and large-scale image retrieval systems. By fully exploiting label annotations, they are achieving outstanding retrieval performances compared to the conventional methods. However, it is painstaking to assign labels precisely for a vast amount of training data, and also, the annotation process is error-prone. To tackle these issues, we propose the first deep unsupervised image retrieval method dubbed Self-supervised Product Quantization (SPQ) network, which is label-free and trained in a self-supervised manner. We design a Cross Quantized Contrastive learning strategy that jointly learns codewords and deep visual descriptors by comparing individually transformed images (views). Our method analyzes the image contents to extract descriptive features, allowing us to understand image representations for accurate retrieval. By conducting extensive experiments on benchmarks, we demonstrate that the proposed method yields state-of-the-art results even without supervised pretraining.

## Concept

<p align="center"><img src="figures/Concept.png" width="900"></p>

By maximizing cross-similarity between the deep descriptor of one view and the product quantized descriptor of the other, both codewords and deep descriptors are jointly trained to contain discriminative image content representations in SPQ.

## An illustration of training procedure in SPQ

<p align="center"><img src="figures/Illustrated_example.png" width="900"></p>

## How to use

### 1. Install requirements on your environment.
- PyTorch=1.7.1
- kornia=0.5.1
- torchvision=0.8.2
- tqdm=4.62.2

### 2. Preparation.
- We utilize CIFAR-10 provide by torchvision in this work.
- We also provide trained model, extract it to the `/path/to/SPQ-master`.
