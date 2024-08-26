# Surgical-Instrument-Segmentation-for-Enhanced-Control-in-RMIS
Surgical Instrument Segmentation for Enhanced Control in RMIS

Paper Link - https://ieeexplore.ieee.org/document/9946418 <br/>
Paper Name - Modified Double U-Net Architecture for Medical Image Segmentation <br/>
Dataset Name : Endovis-2017 <br/>
Dataset Link : https://opencas.dkfz.de/endovis/datasetspublications/ <br/>

𝐏𝐫𝐨𝐣𝐞𝐜𝐭:
The Project aims to increase the accuracy of the network while reducing its size(Trainable Parameters).<br/>
For that i have added using of depthwise convolution layers to reduce the parameters and retaining its accuracy. <br/>
The Modified Double UNET consists of two U-Net's Employed in series, The output of U-Net-1 is paased into U-net-2 and produces a better enhanced segmentation map of the image.<br/>
Basically U-Net is used for medical image segmentation and by using two U-Net's we are trying to increase the accuracy/<br/>
The encoder1 of this network is ensemble of three pretrained networks namely
Inception-V3,MobileNet-V2 and DenseNet-121.<br/>
• Inorder to make the architecture light weight, had employed depthwise seperable
convolutions in encoder and decoder blocks.<br/>
• Squeeze and Excitation attention mechanism is added to skip connections before
concatenating with their respective decoder blocks.<br/>
In Modified Double U-net the Parameters are 29.2 Million whereas the model i have modified has 9 Million parameters which is significant Reduce of 20 Million parameters while retaining accuracy of the model<br/>
In Segementation, the performace of the model can be measured by using <br/>
````Accuracy - 98% <br/>
````Dice Score - 93%<br/>
````IoU Score - 89%<br/>

