# CarND-Semantic Segmentation project
Self-Driving Car Engineer Nanodegree Program

### Project Overview

In this project, we trained a Fully Convolutional Network (FCN) to label the road pixels from images. We started with the VGG16 network and added skip layers, 1x1 convolutions and upsampling to build the FCN.

The test environment: I launch a GPU instances (Instance type p2.xlarge) on Amazon EC2 with the udacity-carnd-advanced-deep-learning AMI from Udacity. After experimented with multiple epochs, batch sizes, learning rates and dropouts hyper parameters during training, finally select the following hyper parameters:

- Epochs: 15
- Batch Size: 16
- Learning rate: 0.0001
- Dropouts: 0.25

### Example Output:

![umm_000041.png](./runs/1503101855.428548/umm_000041.png)

![um_000063.png](./runs/1503101855.428548/um_000063.png)

![uu_000087.png](./runs/1503101855.428548/uu_000087.png)

### Setup
##### Frameworks and Packages
Make sure you have the following is installed:
 - [Python 3](https://www.python.org/)
 - [TensorFlow](https://www.tensorflow.org/)
 - [NumPy](http://www.numpy.org/)
 - [SciPy](https://www.scipy.org/)
##### Dataset
Download the [Kitti Road dataset](http://www.cvlibs.net/datasets/kitti/eval_road.php) from [here](http://www.cvlibs.net/download.php?file=data_road.zip).  Extract the dataset in the `data` folder.  This will create the folder `data_road` with all the training a test images.

### Start
##### Implement
Implement the code in the `main.py` module indicated by the "TODO" comments.
The comments indicated with "OPTIONAL" tag are not required to complete.
##### Run
Run the following command to run the project:
```
python main.py
```
**Note** If running this in Jupyter Notebook system messages, such as those regarding test status, may appear in the terminal rather than the notebook.

### Submission
1. Ensure you've passed all the unit tests.
2. Ensure you pass all points on [the rubric](https://review.udacity.com/#!/rubrics/989/view).
3. Submit the following in a zip file.
 - `helper.py`
 - `main.py`
 - `project_tests.py`
 - Newest inference images from `runs` folder
