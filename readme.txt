-->We are running all codes in Jupyter Notebook.
-->We used python version 3.8.8

-->Libraries Needed for execution of our project:
	import numpy as np
	import pandas as pd 
	import os 
	import cv2 
	import matplotlib.pyplot as plot 
	import keras
	from keras.models import Sequential
	from keras.callbacks import ModelCheckpoint
	from keras.layers import Conv2D, MaxPooling2D, Dense, Flatten, Dropout
	from keras.preprocessing.image import ImageDataGenerator
	from keras.models import load_model
	from PIL import Image
	from tqdm import tqdm
	from pygame import mixer
	import time
        from sklearn.metrics import accuracy_score,classification_report,confusion_matrix
-->Webcam to see your output

-->Description:
Our Project aims at identifying Drivers Drowsiness
We used HaarCascade XML files to identify the face objcets and from that we will identify our eyes action whether they are open or close.
	Reference: https://github.com/opencv/opencv/tree/master/data/haarcascades.
We Downloaded the below xml files from above refence:
   1.haarcascade_frontalface_alt.xml
   2.haarcascade_lefteye_2splits.xml
   3.haarcascade_righteye_2splits.xml
Based on the count score of the closed eye we will blow the alarm to alert the person and prevent from accident. 
To alert the user we used the library below
	from pygame import mixer


Execution of Code:
You need to have the below mentioned model files in the location where we are running our test files.

	1.cnn_keras_drowsiness.h5 
	2.keras_vgg16_drowsiness.h5
Execution:

-->Run the DROWSINESS_DETECTION_WITH_CNN_USING_KERAS_TEST.ipynb file 

Then a video screen will pop up then keep ur eyes closed or open to see the output, if your eye is closed beyond score 16 then alarm will ring and then an image screenshot will be taken.
To quit the screen use 'q'

Similarlly run for vgg16 model also:

-->Run the DROWSINESS_DETECTION_WITH_VGG16_USING_KERAS_TEST.ipynb file

Then a video screen will pop up then keep ur eyes closed or open to see the output, if your eye is closed beyond score 16 then alarm will ring and then an image screenshot will be taken.
To quit the screen use 'q'

For cnn using np_arrays:

-->Run the DROWSINESS_DETECTION_WITH_CNN_USING_np.array.ipynb 
Run the full file, Run the predicted result cell in the notebook that will predict the individual images whether they are open or closed.




