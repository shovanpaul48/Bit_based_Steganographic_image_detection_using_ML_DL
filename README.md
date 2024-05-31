
# Project Title

A brief description of what this project does and who it's for


## Bit based Steganographic image detection using ML

In this project we hide some data in the images, and tried to detcet whether the given image contains some hidden data or not. In this project we use LSB technique to modify the bit and hide data inside the image's pixel bit. We use BossBase dataset for our cover images (this iamges are not doped or steganographic) and mnist dataset  payload iamges (iamegs which are used ad hidden data). 

**Datasets are not availabele in this git repository**


## Tech Stack

**Language:** Python

**Dataset:** Mnist, BossBase

**Platform:** VS Code, Kaggle



## Steps
    1.Downlaod **[BossBase](https://www.kaggle.com/datasets/lijiyu/bossbase)** Dataset

    2.Downlaod **[Mnist](https://www.tensorflow.org/datasets/catalog/mnist)** Dataset

    3.Clean Mnist dataset and store the images in a folder namely "MNIST_NOISEREDUCTION"

    4.Set LSB 1 of Cover images store in a folder "Temp"
    and Set LSB 1 of test cover images store in a folder "Temp_Test" Test cover images 

    5.Split folder "Temp" dataset into 80:20 ratio and store 80 percent iamges in "Stego" 
    and 20 percent images in "Nonstego" folder under "Dataset" folder. Split folder "Temp_test" 
    dataset into 80:20 ratio and store 80 percent iamges in "Test_Stego" and 20 percent 
    images in "Test_Nonstego" folder under "Test_Dataset" folder 

    6.Pick random digit images from "MNIST_NOISEREDUCTION" fodler and hide in iamges from 
    "Stego" Folder and store the steganographic images in another folder "Dataset/Stego"

    7.Define the CNN model

    8.Train the model on "Dataset" folder images 

    9.Save the model

    10.Test the model on "Test_Dataset"


This process takes heavy computing, so we used kaggle's GPU for faster process
 
#### 🔗 [Kaggle notebook Link](https://www.kaggle.com/code/shovansundarpaul/lsb-steganolysis)



In this project we tried Different Bits of the cover image pixel LSB (1th bit), 2nd bit, #3rd bit , and we see after 2nd bit steganography the hidden data can be visible by naked eye 

***LSB steganography***
![Model](https://github.com/shovanpaul48/Bit_based_Steganographic_image_detection_using_ML-/blob/main/New%20folder/bit1.png?raw=true)


***2nd Bit steganography***
![Model](https://github.com/shovanpaul48/Bit_based_Steganographic_image_detection_using_ML-/blob/main/New%20folder/bit2.png?raw=true)


***3rd Bit steganography***
![Model](https://github.com/shovanpaul48/Bit_based_Steganographic_image_detection_using_ML-/blob/main/New%20folder/bit3.png?raw=true)

## Screenshots

**CNN Model Architecture**
![Model](https://github.com/shovanpaul48/Bit_based_Steganographic_image_detection_using_ML-/blob/main/New%20folder/Model_Architecture.png?raw=true)


**Model Training**
![Model](https://github.com/shovanpaul48/Bit_based_Steganographic_image_detection_using_ML-/blob/main/New%20folder/Model_training.png?raw=true)

**Model Test**
![Model](https://github.com/shovanpaul48/Bit_based_Steganographic_image_detection_using_ML-/blob/main/New%20folder/testing_result.png?raw=true)


## Authors

- [@Shovan Sundar Paul](https://github.com/shovanpaul48)



