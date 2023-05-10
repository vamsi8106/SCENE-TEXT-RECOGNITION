# SCENE-TEXT-RECOGNITION
## ABSTRACT
 The field of scene text recognition has become increasingly popular in recent years, as recognizing text in natural scenes presents a significant challenge compared to scanned documents. This paper proposes a novel technique that utilizes first-order Histogram of Oriented Gradient (HOG) through a spatial pyramid,EAST,EASY OCR to address the issue of text recognition in photos of natural scenes and on the internet.Further More,Deep learning-based approaches, such as convolutional neural networks (CNNs) and recurrent neural networks (RNNs), have shown promising results in scene text recognition, and have been combined with various techniques to handle specific challenges, such as attention mechanisms, geometric transformations, and multi-scale processing. The importance of scene text recognition is further underscored by its applications in various domains, including autonomous driving, content-based image retrieval, and cultural heritage preservation.In This paper we have reviewed recent advances in scene text recognition, with a particular focus on deep learning-based methods and their applications.
## Optical Character Recognition
Finding Text In the Scene Images
In other words, OCR software converts a two-dimensional image of text—which could be handwritten or machine printed—into language that a computer can understand. To accomplish OCR as a procedure as accurately as feasible, it typically consists of multiple sub-processes. The subsequent steps are:

1.Preprocessing of the Image  
2.Text Localization  
3.Character Segmentation  
4.Character Recognition  
5.Post Processing  

## Tesseract OCR
Tesseract is an Apache 2.0-licensed open source text recognition (OCR) engine. For programmers, it can be applied directly or through the use of an API to extract written text from photos. Many different languages are supported. Tesseract doesn't come with a built-in graphical user interface, however there are plenty on the 3rdParty website. Through the use of wrappers, which may be obtained here, Tesseract is compatible with a wide range of programming languages and frameworks. It can be used in conjunction with the current layout analysis to find text within a large document or with an outside text detector to find text.

## Methods Implemented
1. EAST
2. EASY OCR
3. FOTS

## 1.EAST
EAST uses a fully convolutional neural network (FCN) to detect text regions in natural scene images. The network is designed to predict the score map and the geometry map of the text regions simultaneously.The score map indicates the likelihood of a pixel being part of a text region, while the geometry map provides information about the shape and orientation of the text region.
### OUTPUT OF EAST METHOD
![wash_east](https://github.com/vamsi8106/SCENE-TEXT-RECOGNITION/assets/99885183/cda692c6-a498-4551-a3b1-14ccd0edda99)

## 2.EASY OCR
Easy OCR is based on deep learning algorithms and pre-trained models that can recognize text in various languages, fonts, and styles.EasyOCR works by first performing image preprocessing to enhance the image quality, such as de-skewing, binarization, and noise reduction.Then, the image is fed into a pre-trained neural network that is capable of recognizing text from the image. The neural network outputs the recognized text along with a confidence score for each character.EasyOCR uses a combination of convolutional neural networks (CNN) and recurrent neural networks (RNN) to recognize text from images.
### OUTPUT OF EASY OCR METHOD
![multi_easy](https://github.com/vamsi8106/SCENE-TEXT-RECOGNITION/assets/99885183/12db4906-f2a9-4f01-bd71-2336dd7ec6c0)

## 3.FOTS
FOTS is an end-to-end trainable framework that detects and recognizes all words in a natural scene image simultaneously. For FOTS we have used ICDAR15 dataset.The overall architecture of FOTS consists of four parts:
1.Shared Convolutions
2.Text Detection Branch
3.RoI Rotate
4.Text Recognition Branch
### OUTPUT OF FOTS METHOD
![fots_text](https://github.com/vamsi8106/SCENE-TEXT-RECOGNITION/assets/99885183/0f7b4fda-28a9-4630-9dad-4ac76c57930f)

## Steps to run the project files
1. Select the Scene text recognition Model as per the required Applications
2. Download the pretrained model weights available online and use them in the code.
3. Use "EASY_OCR_EAST.ipynb" to select the EAST or EASY_OCR model and input image to this model.
4. For FOTS first use "FOTS_Data_Analysis.ipynb" to preprocess the data set
5. Next use "FOTS_Text_Detection_Modelling.ipynb" for finding text in the image.Finally use "FOTS_End_to_End_Modelling.ipnb" to extract text.  
Report Link:   
Youtube Link:https://youtu.be/ThntCvbJrYU  
Custom Data set:https://drive.google.com/drive/folders/1WPx8VuB0pWuWwILQnr9Y44RzeJ56g0Lk?usp=share_link  
## Dependencies
1.OpenCV  
2.Numpy  
3.Matplotlib  
4.pytesseract  
5.easy ocr  
## References
- EASY OCR Reference:https://github.com/nicknochnack/EasyOCR.git
- FOTS Reference:https://towardsdatascience.com/scene-text-detection-and-recognition-using-east-and-tesseract-6f07c249f5de
- FOTS:https://github.com/Vijay-Gadepalli/FOTS.git
- https://github.com/Anugrah-T-Sebastian/Natural-Scene-Text-Recognition.git
