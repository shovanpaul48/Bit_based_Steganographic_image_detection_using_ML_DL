## Bit-based Steganographic Image Detection Using Deep Learning 

In this project, we hide data in images and detect whether a given image contains hidden data or not. We use the LSB (Least Significant Bit) technique to modify the bits and embed data within the image's pixel bits. The BossBase dataset provides our cover images (images without hidden data), and the MNIST dataset supplies payload images (images used as hidden data).

**Note: Datasets are not available in this Git repository.**

## Tech Stack

**Language:** Python

**Datasets:** MNIST, BossBase

**Platform:** VS Code, Kaggle

## Steps

1. Download the **[BossBase](https://www.kaggle.com/datasets/lijiyu/bossbase)** Dataset.
2. Download the **[MNIST](https://www.tensorflow.org/datasets/catalog/mnist)** Dataset.
3. Clean the MNIST dataset and store the images in a folder named "MNIST_NOISEREDUCTION".
4. Set the LSB of the cover images and store them in a folder named "Temp". Similarly, set the LSB of test cover images and store them in a folder named "Temp_Test".
5. Split the "Temp" dataset into an 80:20 ratio, storing 80% of images in the "Stego" folder and 20% in the "Nonstego" folder under the "Dataset" directory. Likewise, split the "Temp_Test" dataset into an 80:20 ratio, storing 80% of images in the "Test_Stego" folder and 20% in the "Test_Nonstego" folder under the "Test_Dataset" directory.
6. Randomly pick digit images from the "MNIST_NOISEREDUCTION" folder and hide them in images from the "Stego" folder. Store the steganographic images in the "Dataset/Stego" folder.
7. Define the CNN model.
8. Train the model on the "Dataset" folder images.
9. Save the model.
10. Test the model on the "Test_Dataset" images.

This process is computationally intensive, so we used Kaggle's GPU for faster processing.

#### 🔗 [Kaggle Notebook Link](https://www.kaggle.com/code/shovansundarpaul/lsb-steganolysis)

In this project, we experimented with different bits of the cover image pixel LSB (1st bit, 2nd bit, 3rd bit). We observed that after the 2nd bit, the hidden data becomes visible to the naked eye.

### Examples of LSB Steganography

**LSB (1st bit) Steganography**

![1st Bit Steganography](https://github.com/shovanpaul48/Bit_based_Steganographic_image_detection_using_ML-/blob/main/New%20folder/bit1.png?raw=true)

**2nd Bit Steganography**

![2nd Bit Steganography](https://github.com/shovanpaul48/Bit_based_Steganographic_image_detection_using_ML-/blob/main/New%20folder/bit2.png?raw=true)

**3rd Bit Steganography**

![3rd Bit Steganography](https://github.com/shovanpaul48/Bit_based_Steganographic_image_detection_using_ML-/blob/main/New%20folder/bit3.png?raw=true)

## Screenshots

**CNN Model Architecture**

![Model Architecture](https://github.com/shovanpaul48/Bit_based_Steganographic_image_detection_using_ML-/blob/main/New%20folder/Model_Architecture.png?raw=true)

**Model Training**

![Model Training](https://github.com/shovanpaul48/Bit_based_Steganographic_image_detection_using_ML-/blob/main/New%20folder/Model_training.png?raw=true)

**Model Testing**

![Model Testing](https://github.com/shovanpaul48/Bit_based_Steganographic_image_detection_using_ML-/blob/main/New%20folder/testing_result.png?raw=true)

## Authors

- [@Shovan Sundar Paul](https://github.com/shovanpaul48)
