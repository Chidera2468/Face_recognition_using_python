# Building a face detection and recognition tool with python
INTRODUCTION
This project helps its users to build face detection and recognition tool using Python. I am the only contributor to this project. As a software engineer I am focusing on building a face recognition tool that could help companies and other vital bodies in the society, especially in the area of security and transportation.
The level of insecurity in my area is becoming overwhelming. I was on the streets one day when I saw some unknown gunmen walk out of their cars just to rob different shops of their hard-earned money without being disturbed or recognized. When the victims affected by the ugly incident are asked if they could recognize these people they usually gave a negative answer. This issue of robbery continued to the extent that I got worried and I asked myself the reason I am in this world. I discovered that one of the reasons for existence on Earth is to solve problems. I started looking for a way to solve this problem of insecurity. I realized that this project will help me find a solution to this problem of insecurity. I hope to use this tool to help reduce the level of insecurity and capture the faces of those who are guilty of crimes.
Below are links to my linkedIn and blog article;
https://medium.com/@chidera2468/face-recognition-tool-with-python-b685da043805
https://www.linkedin.com/in/chidera-jamike-947363270/

[![PyPI](https://badge.fury.io/py/FaceReco.png)](https://pypi.org/project/FaceReco/)

## Installing
pip install FaceReco

## Description
Face Recognition is a very popular topic. It has lot of use cases in the filed of biometric security. 
Now a days with the help of Deep learning face recognition has become very feasible to people. 
As deep learning is a very data intensive task and we may always not have such huge amount of data to work in case of face recognition 
so with the advancement in One Shot Learning, face recognition has become more practical and feasible. This Python Package make it even more feasible, simple 
and easy to use. We have eliminated all the steps to download the supporting files and setting up the supporting files. You can simply installed the python package and start doing face detection and recognition.

## Steps Explanation
To learn more about the tasks which are being performed on the backend head over to link : [Step by Step Face Recognition Code Implementation From Scratch In Python](https://towardsdatascience.com/step-by-step-face-recognition-code-implementation-from-scratch-in-python-cc95fa041120)

## Using The Package

#### Train Model

```python
import FaceReco.FaceReco as fr
fr_object1 =  fr.FaceReco()
fr_object1.train_model("lfw_selected/face")
``` 

#### Test Model

```python
fr_object1.test_model("lfw_selected/face2/Johnny_Depp_0002.jpg")
``` 

#### Load Saved Model

```python
fr_object2 =  fr.FaceReco()
fr_object2.load_model("Model_Object_1") #folder of saved model
fr_object2.test_model("lfw_selected/face2/Johnny_Depp_0002.jpg")
``` 
