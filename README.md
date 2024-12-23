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
- [Key Findings](#key-findings)
- [Links to Resources](#links-to-resources)

## Deep Models

### DAE-Former
Dual Attention-guided Efficient Transformer (DAE-Former) is a pure Transformer-based U-shape architecture designed for medical image segmentation. This architecture incorporates three types of attention mechanisms: (1) efficient attention, (2) transpose attention, and (3) cross attention. Dual-attention blocks were capturing both spatial and channel information by incorporating efficient attention and transpose attention. Skip-connection cross-attention (SCCA) was employed to suppress irrelevant regions in the image during training and highlight significant features for the segmentation task.

<img src="images/DAE-Former.jpg" width="30%" height="30%">

### LKA and DLKA
<img src="images/DLKA-blocks.jpg" width="30%" height="30%">


### FCT

<img src="images/FCT.jpg" width="80%" height="80%">


### nnU-Net
<img src="images/nnUNet.jpg" width="70%" height="70%">


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

<img src="images/ISLES-table.png" width="100%" height="100%">
<img src="images/ISLES22.png" width="100%" height="100%">

### <a name="atlas_results"></a> ATLAS v2.0

<img src="images/ATLAS-table.png" width="100%" height="100%">
<img src="images/ATLAS.png" width="100%" height="100%">

##  Key Findings
- The nnU-Net, with its simple architecture, outperformed more complex models.
- Local information captured by CNN layers is highly informative and cannot be fully replaced by the global features provided by Transformers for stroke segmentation.
- Pre- and post-processing steps are critical and should not be overlooked in favor of solely architectural design.
- Transformers face challenges when handling imbalanced data distributions, such as variations in the number of lesions per slide.
- A thoughtful integration of CNN layers and Transformers is crucial for enhancing the performance of deep models in stroke segmentation.
  
## Links to Resources
- [DAE-Former Repository](https://github.com/xmindflow/DAEFormer)
- [LKA/DLKA Repository](https://github.com/xmindflow/deformableLKA)
- [FCT Repository](https://github.com/Thanos-DB/FullyConvolutionalTransformer)
- [nnU-Net Repository](https://github.com/MIC-DKFZ/nnUNet)
- [ISLES 2022 Dataset](https://isles22.grand-challenge.org/)
- [ATLAS v2.0 Dataset](https://atlas.grand-challenge.org/)
