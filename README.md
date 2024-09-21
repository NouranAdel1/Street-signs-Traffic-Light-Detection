# Street Signs and Traffic Light Detection Using YOLOv5 and Roboflow Dataset

## Overview
This project focuses on detecting street signs and traffic lights (red and green) using the YOLOv5 model. YOLOv5 is a state-of-the-art object detection algorithm, trained using a dataset from Roboflow that contains annotated images of various road signs.

## Dataset
The dataset used for training can be found on Roboflow:
[Roboflow Road Signs Dataset](https://universe.roboflow.com/roboflow-100/road-signs-6ih4y/dataset/2).

## Model
The object detection model is built using YOLOv5, developed by Ultralytics. More information, including setup instructions, is available on their GitHub repository:
[YOLOv5 GitHub Repository](https://github.com/ultralytics/yolov5).

The repository also includes:
- A **Jupyter Notebook (.ipynb)** to walk through the training and testing process.
- A **presentation** summarizing the project, the challenges faced, and the solutions implemented.

## Challenge
Initially, the YOLOv5 model encountered difficulties in accurately detecting road signs. This was due to suboptimal training settings, resulting in poor classification of street signs and traffic lights.

## Solution
To improve detection accuracy, the following training parameters were adjusted:
- **Image Size**: Resized all input images to 640x640 pixels.
- **Batch Size**: Set the batch size to 16.
- **Epochs**: Increased the number of training epochs to 100.
- **Hyperparameters**: Fine-tuned the model using a custom configuration file for better optimization.

These adjustments led to a significant improvement in model performance, allowing it to detect road signs and traffic lights with much higher accuracy.

## Improvements
- **Better Detection Accuracy**: Improved detection of various road signs and accurate identification of red and green traffic lights.
- **Optimized Training**: Fine-tuning the parameters significantly boosted model performance.

## Testing the Model
The trained model was tested on two videos to demonstrate its real-time detection capabilities. Below are the results:

### Test 1: Video Detection
- Input: A video of a car moving through a road with Road Signs.
- Output: 
<center>
  <img src="https://github.com/NouranAdel1/Street-signs-Traffic-Light-Detection/blob/main/Test_Demo1.gif" width="300">
</center>

### Test 2: Video Detection
- Input: A different video of a POV of walking through a park with Road Signs .
- Output:
<center>
  <img src="https://github.com/NouranAdel1/Street-signs-Traffic-Light-Detection/blob/main/Test_Demo2.gif" width="300">
</center>

### Test 3: Picture Detection
- Input: Test picture of a traffic light (Red or Green) .
- Output:
<center>
  <img src="https://github.com/NouranAdel1/Street-signs-Traffic-Light-Detection/blob/main/TrafficLight_Picture_test.jpg" width="300">
</center>

## Conclusion
The YOLOv5 model, trained with the Roboflow dataset, now demonstrates high accuracy in detecting road signs and traffic lights. This makes it suitable for use in real-world applications like autonomous driving, traffic monitoring, and road safety systems.


