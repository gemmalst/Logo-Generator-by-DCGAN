# AI Logo Generator Using DCGAN

<p align="center">
  <img width="267" height="317" src="logol.png">
</p>


## LOGOL - Xccelerate Data Science and Machine Learning Capstone Project
LOGO⅃ is an AI logo generator that aims creating large amount of quality logos within seconds and providing alternative solutions for advertising as well as creative industries. Through using LLD dataset provided for establishing the prototype of different GAN models in the early stage of our project for trial purposes to see the differences among the GANs while later obtaining over 365k logos from App Store to training our final DCGAN model, we have suceeded in creating an user-friendly and instant logo generator through deep learning model.



## Data Collection

#### - LLD Large Logo Dataset

<a href="https://data.vision.ee.ethz.ch/cvl/lld/">LLD dataset</a> [1] contains various logo dataset with different amount and resolution of logo in which we have chosen two of the datasets provided:

1.   **5,000** logos with low resolution (32x32)

2.   **122,920** logos with high resolution (400x400)


#### - 365k IOS Apps Dataset

<a href="https://www.kaggle.com/fentyforte/365k-ios-apps-dataset">365k IOS Apps Dataset</a> [2] is created by us using Rapid API to acquire the data we need and we have scraped over 10,000,000 but we have filtered out the data rows with incomplete information so there are only 365k data left. We have used 5 Jupyter Notebooks at the same time to scrape thus download the logos which took us around 2 days using the Macbook Pro (specification mentioned below).

## Model Architectural Diagram

<p align="center">
  <img src="model_architecture.png">
</p>


## Results 

<table>
  <tr>
    <th>DCGAN with 120k img</th>
    <th>DCGAN with 58k img (Games Category)</th>
  </tr>
  <tr>
    <th><img src="120k.gif"></th>
    <th><img src="dcgan_game.gif"></th>
  </tr>
  
</table>

### Specifications & Time 
<br>
We have scaled down 365,915 images from 512x512 pixels to 64x64 pixels for training our DCGAN model due to our limited computational power and financial status.<br>
The following are the specifications of computer/VM instances & time used for training DCGAN:<br><br><br>

### **MacBook Pro** <br><br>
**CPU**: 2.3GHz 8-Cppre Intel Core i9 <br>
**RAM**: 32 GM 2667 MHz DDR4 <br>
**Graphic Card**: Intel UHD Graphics 630 1536MB <br><br>

**Time Required**(120k):<br>
100 epochs/96100 iterations with 120k images: ~**4.25** days <br>
1 epoch/961 iterations: ~**3800-4200** seconds <br>
1000 iterations: ~**4200-4400** seconds <br><br>

### **GCP AI VM Instances** <br><br>
**Environment**: PyTorch 1.6 <br>
**Machine Type**: 4 vCPUs, 15 GB RAM <br>
**GPUs**: NVIDIA Tesla T4 x 1 <br>

**Time Required**(365k):<br>
100 Epochs/ 285800 Iterations: ~**5990** seconds <br>
1 epoch/2858 iterations: ~**666** seconds <br>
1000 iterations: ~**233** seconds <br><br>



#### DCGAN


## Limitations


## Pitch
-------show pitch here rmb edit arr on9999--------

## References
1. LLD Dataset - https://data.vision.ee.ethz.ch/cvl/lld/
2. 365k IOS Apps Dataset - https://www.kaggle.com/fentyforte/365k-ios-apps-dataset
3. 365k IOS Apps Logos Dataset - 

https://medium.com/analytics-vidhya/conditional-icon-generation-with-gans-2cc489e23d9a
