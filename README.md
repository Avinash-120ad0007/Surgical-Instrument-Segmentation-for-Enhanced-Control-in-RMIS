# Surgical-Instrument-Segmentation-for-Enhanced-Control-in-RMIS
Surgical Instrument Segmentation for Enhanced Control in RMIS

Paper Link - https://ieeexplore.ieee.org/document/9946418 <br/>
Paper Name - Modified Double U-Net Architecture for Medical Image Segmentation <br/>
Dataset Name : Endovis-2017 <br/>
Dataset Link : https://opencas.dkfz.de/endovis/datasetspublications/ <br/>


## Overview

This project aims to enhance the accuracy of medical image segmentation while significantly reducing the network's size (trainable parameters). The architecture is based on a Modified Double U-Net, consisting of two U-Net networks employed in series. The output of U-Net-1 is passed into U-Net-2 to produce a more refined segmentation map of the image.

## Key Features

1. **Depthwise Convolution Layers:** 
   - To reduce the number of parameters and retain accuracy, depthwise separable convolutions have been employed in both encoder and decoder blocks.

2. **Modified Double U-Net Architecture:**
   - The architecture utilizes two U-Nets in series to improve segmentation accuracy.
   - U-Net is commonly used for medical image segmentation, and by stacking two U-Nets, we aim to further enhance accuracy.

3. **Encoder Composition:**
   - The encoder1 of the network is an ensemble of three pretrained networks: Inception-V3, MobileNet-V2, and DenseNet-121. This combination helps in capturing various features efficiently.

4. **Attention Mechanism:**
   - A Squeeze and Excitation attention mechanism is added to the skip connections before concatenating them with their respective decoder blocks. This mechanism improves the network's ability to focus on relevant features.

5. **Model Size and Performance:**
   - The original Modified Double U-Net has 29.2 million parameters. After optimization, the model has only 9 million parameters, reducing the size by 20 million parameters while maintaining accuracy.
   - Performance metrics:
     - **Accuracy:** 98%
     - **Dice Score:** 93%
     - **IoU Score:** 89%

## Conclusion

This project demonstrates that by employing depthwise separable convolutions, ensemble learning, and attention mechanisms, we can significantly reduce the number of parameters in a segmentation model without compromising its accuracy. The Modified Double U-Net provides an effective and efficient solution for medical image segmentation tasks.


