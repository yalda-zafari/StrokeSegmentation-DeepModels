# <p align=center>`Deep Models for Stroke Segmentation: Do Complex Architectures Always Perform Better?`</p> #

This repository summarizes the results of our paper, "Deep Models for Stroke Segmentation: Do Complex Architectures Always Perform Better?" The paper evaluates the effectiveness of various deep learning models for stroke lesion segmentation and explores whether complex architectures consistently outperform simpler designs.

## Updates
- Initial release on arXiv: [Deep models for stroke segmentation: do complex architectures always perform better?](https://arxiv.org/abs/2403.17177)
- Our review paper on Artificial Intelligence Review: [Transformers-based architectures for stroke segmentation: a review](https://link.springer.com/article/10.1007/s10462-024-10900-5)


## Table of Content
- [Deep Models](#deep-models)
  - [DAE-Former](#dae-former)
  - [LKA and DLKA](#lka-and-dlka)
  - [FCT](#fct)
  - [nnU-Net](#nnu-net)
- [Datasets](#datasets)
- [Results](#results)
  - [ISLES 2022](#isles_results)
  - [ATLAS v2.0](#atlas_results)
- [Key Outcomes](#key-outcomes)
- [Links to Resources](#links-to-resources)

## Deep Models

### DAE-Former

### LKA and DLKA

### FCT

### nnU-Net

## Datasets
We used two publicly accessible datasets for stroke segmentation to ensure sufficient data diversity and volume for training deep neural networks:

1. ISLES 2022:
  - Contains 400 MRI cases (250 public, 150 private).
  - Features diverse infarct patterns and imaging from three medical centers.
  - Includes DWI, ADC, and FLAIR modalities (we used DWI images only).

2. ATLAS v2.0:
  - Includes 955 T1-weighted MRI cases (655 public with lesion masks, 300 without).



## Results

### <a name="isles_results"></a> ISLES 2022

### <a name="atlas_results"></a> ATLAS v2.0

##  Key Outcomes

## Links to Resources
- [DAE-Former Repository](https://github.com/xmindflow/DAEFormer)
- [LKA/DLKA Repository](https://github.com/xmindflow/deformableLKA)
- [FCT Repository](https://github.com/Thanos-DB/FullyConvolutionalTransformer)
- [nnU-Net Repository](https://github.com/MIC-DKFZ/nnUNet)
- [ISLES 2022 Dataset](https://isles22.grand-challenge.org/)
- [ATLAS v2.0 Dataset](https://atlas.grand-challenge.org/)
