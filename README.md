# Cyclist Object Detection
By Rohan Kelley and Vincent Tinaro

## Brief Description
In an attempt to learn more about Neural Networks and the utilities behind them, we came up with a plan to conduct research and create a neural network that can identify cyclists and draw a bounding box around them. 

## The Data
We obtained the [data](https://www.kaggle.com/datasets/semiemptyglass/cyclist-dataset/data) via kaggle, and found that it contained around 13,700 images each with dimensions 2048 x 1024, and each image had an associated text file with the yolo label which documented the bounding box annotations. 

## Implementation
Utilized the YOLOv8 model from keras, and had our data in the form of a tensorflow Dataset object. More details found in the [report](Project%20Final%20Report.pdf) and in the [code](ML_Object_Detection_Project_Final.ipynb) itself.

## Results
Overall, our model had alright accuracy. We utilized a combined F1 score (provides a balanced measure of the model’s performance in the terms of both the bounding box prediction and classification), and received this score to be 0.732. While not perfect, these are still positive results as the model did learn the bounding box classifications, and these results can be improved upon in the future.

Here are some example images:
--------
![Example Prediction 1](https://github.com/Rohank12/cyclist-detection/blob/main/Screenshot%202023-12-19%20150853.png)
![Example Prediction 2](https://github.com/Rohank12/cyclist-detection/blob/main/Screenshot%202023-12-19%20150912.png)
![Example Prediction 3](https://github.com/Rohank12/cyclist-detection/blob/main/Screenshot%202023-12-19%20150929.png)
