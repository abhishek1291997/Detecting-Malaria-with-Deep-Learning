# Detecting-Malaria-with-Deep-Learning
Here is the way to detect malaria by their cell images

This code pattern demonstrates how images, specifically cell images of Parasitized and Uninfected can be classified using Convolutional Neural Network (CNN).

**Let's talk something about malaria**
Malaria is a life-threatening disease caused by parasites that are transmitted to people through the bites of infected female Anopheles mosquitoes. It is preventable and curable. According to WHO there are 212 Million malaria cases and 435000 deaths. Early diagnostics and treatment of malaria can prevent deaths. Malaria is prevalent across the world especially in tropical regions the severity of malaria varies based on the species of plasmodium. Symptoms are chills, fever and sweating, usually occurring a few weeks after being bitten.

## Why CNN for malaria detection? 
Convolution layers learn spatial hierarchical patterns from the data, which are also translation invariant. Thus they are able to learn different aspects of images. For example, the first convolution layer will learn small and local patterns such as edges and corners, a second convolution layer will learn larger patterns based on the features from the first layers, and so on. This allows CNNs to automate feature engineering and learn effective features which generalize well on new data points. Pooling layers help with downsampling and dimension reduction.
Thus, CNNs help us with automated and scalable feature engineering. Also, plugging in dense layers at the end of our model enables us to perform tasks like image classification. Automated malaria detection using deep learning models like CNNs could be very effective, cheap and scalable especially with the advent of transfer learning and pre-trained models which work quite well even with constraints like less data.

## Getting Started
Use the Anaconda navigator to open the Jupyter notebook and start implementing it.

## Pre-requisites 
**Install all these libraries in your local environment**
* Numpy
* Pandas
* Scikit-learn
* Keras
* cv2
* pathlib
* glob
* os

### Dataset
The dataset contains 2 folders - Infected - Uninfected

And a total of 27,558 images.

## Working
- Firstly, I imported all the useful libraries needed for our project. Then we started by creating empty lists for our training data, test data folder.
- After all this, get all the images from directories to predefined empty lists, by reading them and resizing them so that all the images are of same size. After this, start making the model and training the data.
- The main **challenge** faced while making this project is less amount of data, because this is the technology which is useful in near future to detect the malaria by AI, so we need to be accurate as much as possible.
- For this we used **Data Augmentation** to used the current data we have to generate more data which is much more feasible.

## Acknowledgements
This Dataset is taken from the official NIH Website: https://ceb.nlm.nih.gov/repositories/malaria-datasets/ And uploaded here, so anybody trying to start working with this dataset can get started immediately, as to download the dataset from NIH website is quite slow.

Photo by Егор Камелев on Unsplash https://unsplash.com/@ekamelev

### Inspiration
Save humans by detecting and deploying Image Cells that contain Malaria or not!
