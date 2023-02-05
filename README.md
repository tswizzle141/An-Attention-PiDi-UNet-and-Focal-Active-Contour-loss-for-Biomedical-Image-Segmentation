# An-Attention-PiDi-UNet-and-Focal-Active-Contour-loss-for-Biomedical-Image-Segmentation
#### (Specially thanks to @minhnhattrinh312 for our lovely cooperation)
## Introduction
MRI cardiac segmentation on the [ACDC](https://www.creatis.insa-lyon.fr/Challenge/acdc/databases.html) (3-D images), Skin Lesion segmentation on [ISIC 2018](https://challenge.isic-archive.com/landing/2018/45/) (2-D images), Skin Cancer segmentation on [PH2](https://www.fc.up.pt/addi/ph2%20database.html) (2-D images).
## Our contributions
![Proposed Model](https://github.com/tswizzle141/An-Attention-PiDi-UNet-and-Focal-Active-Contour-loss-for-Biomedical-Image-Segmentation/blob/main/1.jpg)
* Influenced by the ConvMixer layer, we have created a residual operation after the depthwise layer before feature maps are fed into the pointwise layer. Nevertheless, instead of utilizing GeLU activation, we have still used the ReLU activation.
