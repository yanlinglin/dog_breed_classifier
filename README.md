[//]: # (Image References)

[image1]: ./images/sample_dog_output.png "Sample Output"
[image2]: ./images/vgg16_model.png "VGG-16 Model Keras Layers"
[image3]: ./images/vgg16_model_draw.png "VGG16 Model Figure"


## Project Overview

This project is the capestone project of Udacity Data Scientist Nanodegree. In this project, you will learn how to build a pipeline that can be used within a web or mobile app to process real-world, user-supplied images.  Given an image of a dog, your algorithm will identify an estimate of the canine’s breed.  If supplied an image of a human, the code will identify the resembling dog breed.  

![Sample Output][image1]

### the motivation for the project, 

Along with exploring state-of-the-art CNN models for classification, you will make important design decisions about the user experience for your app.  Our goal is that by completing this lab, you understand the challenges involved in piecing together a series of models designed to perform various tasks in a data processing pipeline.  Each model has its strengths and weaknesses, and engineering a real-world application often involves solving many problems without a perfect answer.  Your imperfect solution will nonetheless create a fun user experience!



## Project Instructions

### Instructions

1. Clone the repository and navigate to the downloaded folder.
```	
git clone https://github.com/udacity/dog-project.git
cd dog-project
```

2. Download the [dog dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip).  Unzip the folder and place it in the repo, at location `path/to/dog-project/dogImages`. 

3. Download the [human dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip).  Unzip the folder and place it in the repo, at location `path/to/dog-project/lfw`.  If you are using a Windows machine, you are encouraged to use [7zip](http://www.7-zip.org/) to extract the folder. 

4. Donwload the [VGG-16 bottleneck features](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogVGG16Data.npz) for the dog dataset.  Place it in the repo, at location `path/to/dog-project/bottleneck_features`.

## The libraries used

This project used Keras extensively for creating the CNN. The following packages are used:
- numpy: handling training, validation and testing data;
- matplotlib: plot images; 
- pandas: showing the class distribution of provided data;
- cv2: processing and showing images 
- tqdm: showing progress bar.


## files in the repository with a small description of each:
- dog_app.ipynb: contains the main code and results of the project.
- extract_bottleneck_features.py: The functions to extract the bottleneck features can be found in extract_bottleneck_features.py. To obtain the bottleneck features corresponding to your chosen CNN architecture, you need to use the function extract_{network} where {network}, in the above filename, should be one of VGG19, Resnet50, InceptionV3, or Xception.


## A summary of the results of the analysis
In the project, a built-from-scratch CNN model, three transfer-learning based models based on VGG16, VGG19 and ResNet 50. Their test accuracy is reported below:
- built-from-scratch CNN: 10.6459%
- VGG16-based model:      44.6172%
- VGG19-based model:      74.4019%
- ResNet50-based model:   80.3827%



## Acknowledgements. 
This project is provided by Udacity Data Scientist Nanodegree. Some parts of this readme file is from the Udacity project description and code. 

