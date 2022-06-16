# QFormer
A highly-efficient Quaternion Transformer (QFormer) for image denoising. If this paper is accepted, the code will be released as soon as possible.

## Abstract
Since Deep Convolutional Neural Networks (DCNNs) and Vision Transformer perform well in learning generalizable image priors from large-scale data, these models have been widely used in image denoising tasks. However, vanilla DCNNs and Transformer suffer from two problems. First, the vanilla DCNNs and Transformer only accumulate the output along the channel axis, ignoring the internal relationship among channels. This results in the severely inadequate color structure representation retrieved from color images. Secondly, the DCNNs or Transformer-based image denoising models usually have a large number of parameters, high computational complexity, and slow inference speed. To resolve these issues, this paper proposes a highly-efficient Quaternion Transformer (QFormer) for image denoising. Specifically, the proposed Quaternion Transformer Block (QTB) simplifies the typical Transformer from a multi-branch structure to an elaborately sequential structure mainly with quaternion transformations, to alternately capture both long-range dependencies and local contextual features with color structure information. Furthermore, the proposed QTB can also avoid considerable element-wise multiplications of computing the self-attention matrices. Thus, our QTB can significantly reduce the computational complexity and its sequential structure can further improve the practical inference speed. Comprehensive experiments demonstrate that the proposed QFormer produces state-of-the-art results in both denoising performance and efficiency. We hope that our work will encourage further research to explore the Quaternion Transformer architecture for image denoising tasks.

## Overall structure of the proposed QFormer Network
![avatar](https://github.com/JiangBoCS/QFormer/blob/main/xuanzhuan.png)

![avatar](https://github.com/JiangBoCS/QFormer/blob/main/P-S.png)
PSNR value and the number of parameters on the real noisy image testing sets. (a) on the SSID dataset. (b) on the PolyU dataset. (c) on the Nam dataset.
