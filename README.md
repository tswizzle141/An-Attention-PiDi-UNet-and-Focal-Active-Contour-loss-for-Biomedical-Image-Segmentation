# An-Attention-PiDi-UNet-and-Focal-Active-Contour-loss-for-Biomedical-Image-Segmentation
#### (Specially thanks to @minhnhattrinh312 for our lovely cooperation)
See the [pdf](https://ieeexplore.ieee.org/document/10013852) here.
## Introduction
MRI cardiac segmentation on the [ACDC](https://www.creatis.insa-lyon.fr/Challenge/acdc/databases.html) (3-D images), Skin Lesion segmentation on [ISIC 2018](https://challenge.isic-archive.com/landing/2018/45/) (2-D images), Skin Cancer segmentation on [PH2](https://www.fc.up.pt/addi/ph2%20database.html) (2-D images).
## Our contributions
![Proposed Model](https://github.com/tswizzle141/An-Attention-PiDi-UNet-and-Focal-Active-Contour-loss-for-Biomedical-Image-Segmentation/blob/main/1.jpg)
* Influenced by the ConvMixer layer, we have created a residual operation after the depthwise layer before feature maps are fed into the pointwise layer. Nevertheless, instead of utilizing GeLU activation, we have still used the ReLU activation.
* Starting from the end of each decoder stage, a CDCM is proposed for boundary refinement. A Map Reduce, which is $1 \times 1$ convolutional layer, scales down the feature map into a single channel map for further interpolation and concatenation to the original size of the input image. We have observed that the CDCM output channel could be adjusted among values of the set containing the power of 2 $({1,2,4,8,16})$; the segmentation result of each dataset varies when this value changes.
