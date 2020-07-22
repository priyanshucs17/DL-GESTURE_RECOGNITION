# DL-GESTURE_RECOGNITION
## Problem Statement:
Imagine you are working as a data scientist at a home electronics company which manufactures state of the art __smart televisions__. You want to develop a cool feature in the smart-TV that can __recognise five different gestures__ performed by the user which will help users control the TV without using a remote.

#### The gestures are continuously monitored by the webcam mounted on the TV. Each gesture corresponds to a specific command:
-> __Thumbs up__:  Increase the volume

-> __Thumbs down__: Decrease the volume

-> __Left swipe__: 'Jump' backwards 10 seconds

-> __Right swipe__: 'Jump' forward 10 seconds  

-> __Stop__: Pause the movie

-> Each video is a sequence of __30 frames (or images)__.

## Understanding the Dataset:
The training data consists of a few hundred videos categorised into one of the five classes. Each video (typically 2-3 seconds long) is divided into a __sequence of 30 frames(images)__. These videos have been recorded by various people performing one of the five gestures in front of a webcam - similar to what the smart TV will use. 

The data is in a zip file. The zip file contains a '__train__' and a '__val__' folder with __two CSV files for the two folders__. These folders are in turn divided into subfolders where each subfolder represents a video of a particular gesture. Each subfolder, i.e. a video, contains 30 frames (or images). Note that all images in a particular video subfolder have the same dimensions but different videos may have different dimensions. Specifically, videos have two types of dimensions - either __360x360 or 120x160__ (depending on the webcam used to record the videos). Hence, you will need to do some pre-processing to standardise the videos. 

Each row of the CSV file represents one video and contains three main pieces of information - the name of the subfolder containing the 30 images of the video, the name of the gesture and the numeric label (between 0-4) of the video.

Your task is to train a model on the '__train__' folder which performs well on the '__val__' folder as well (as usually done in ML projects). We have withheld the test folder for evaluation purposes - your final model's performance will be tested on the 'test' set.



PGDML_CASE-STUDY
