# DSND: Dog Breed Classifier

## Table of Contents

1. [Project Motivation](#motivation)
2. [File Descriptions](#files)
3. [Results](#results)
4. [Required Libraries](#libraries)


## Project Motivation <a name="motivation"></a>

The purpose of this project is to use a convolutional neural network (CNN) to predict dog breeds. The model could be used as part of a mobile or web app, as it accepts any user-supplied image as input. 
If a dog is detected in the image, it will estimate the dog's breed. If a human is detected, it will provide the resembling dog breed.


## File Descriptions <a name="files"></a>
- dog_app.ipynb is a Jupyter notebook, which contains the entire project code that was used to create a dog breed classifier.
- The 'images' folder includes all images used for this project.
- The 'saved_models' folder contains models that were saved during this project

## Results <a name="results"></a>

n summary, the performance of the pre-trained model I built far exceeded the hand made CNN model. The accuracy of the InceptionV3 model (pre-trained on ImageNet) exceeded 80% while the CNN from scratch was under 4%.
This improved performance can be attributed to the vast dataset on which the pre-trained model was built. The ImageNet dataset contains more than one million training images on which the InceptionV3 model was trained, hence an extreme increase in performance as compared to CNN from scratch. 
When tested on new images, the CNN model with transfer learning performed as expected: not perfect, but good enough. 


## Required Libraries <a name="libraries"></a>

- Pandas, NumPy, Scikit-learn (Machine Learning Libraries)
- Matplotlib (Plotting library)
- Keras (Neural-network library)
- Glob library 

Inception bottleneck features can be downloaded here: https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogInceptionV3Data.npz
<br>The summary can be found in my article here: https://ttikh.medium.com/from-dogs-to-classifiers-2baf495e6a27
