# Pestdetection
**Welcome to the Pestdetection wiki!**

###  PEST DETECTION USING IMAGE PROCESSING
e-yantra Ideas Competition - 2017
 
 Abstract
The principal idea which empowered us to work on the project PEST DETECTION USING IMAGE PROCESSING is to ensure improved and better farming techniques for farmers.

Present Scenario:
The present scenario in the agricultural field is not proficient enough as the farmers have to face a lot of problems like survey the land manually for pest detection.So, to alleviate such problems we came up with this very idea.

Our Solution:
The techniques of image analysis are extensively applied to agricultural science, and it provides maximum protection to crops and also much less use of pesticides which can ultimately lead to better crop management and production. Monitoring of pests infestation relies on manpower, however automatic monitoring has been advancing in order to minimize human efforts and errors.
 
 Introduction/Motivation
Most of the farmers used the traditional pest management methods which is the regular spray program which sometimes kill useful insects that help in eradicating pests.The old methods trap the insect pests and are brought to the laboratory for counting  and identifying manually which are used to estimate the pest density.However this process is tedious and time consuming for a crop technician and also lead to low count accuracy and delays in obtaining accurate counts. Due to the rapid development of digital technology, there is an opportunity for image processing technology to be used  of agricultural research which could help the researcher to solve a complex problem. Image analysis provides a realistic opportunity for the automation of insect pest detection. Through this system, crop technicians can easily count the pests from the collected specimens, and right pests’ management can be applied to increase both the quantity and quality of  production. Using the automated system, crop technicians can make the monitoring process easier. 
This motivates us to choose this project as a means to help farmers in their work.
 
Literature Survey/Prior Artwork
 > Early Pest Detection from Crop using Image Processing and Computational Intelligence by Danish Gondal and Yasir Naiz,Their paper proposed a framework for early detection of pests.
 
Reference-https://www.researchgate.net/publication/282119578_Early_Pest_Detection_from_Crop_using_Image_Processing_and_Computational_Intelligence
> e-Sagu: An IT based Personalized Agro-Advisory System- This system provided the farmers with the mobile phones to take the pictures of their crops themselves and then it goes to the nearest e-sagu center for the report generation which is again a tedious task to do.
Reference-https://youtu.be/YFvGvr3vzIw
 
 
 Hardware Requirement
The following are the hardware requirements for the project:
 
 IP Camera module : To capture and transfer the image
Arduino : A microcontroller which will do the following functions: hover, obstacle sensing and path determination
SD Card :  to save the captured images and further can be inserted in a mobile or a laptop
Brushless Motors,Propeller Set : Flying the drone
Multi Copter Frame : A frame for the drone
A laptop/Android mobile : For report analysis
 
 
  Software Requirement
The following softwares are required for the project:
 
OpenCV with C++/Python : It is a library which is designed for computational efficiency with a strong focus on real time applications.
Arduino IDE : The open-source Arduino Software (IDE) makes it easy to write code and upload it to the board. It runs on Windows, Mac OS X, and Linux. The environment is written in Java and based on Processing and other open-source software. This software can be used with any Arduino board.
 
 
 
 Implementation
 
The System is divided into following sub heads -
 
Importing the image by digital processing using IP camera module(IMAGE ACQUISITION) 
Transmitting it to the laptop through SD Card
Analysing the image using OpenCV
Report based on image analysis
 
Image captured by the IP Camera boarded on the Arduino Controlled Flying Drone is sent to the laptop using wifi/bluetooth. Once the Image Acquisition is done, its analysis is done using OpenCV. 
 
Analysis using OpenCV is further divided into the following sub head : 
 
 Pest Detection System
Following are the image processing steps which are used in the proposed system.
>Color Image  to Gray Image Conversion
Therefore,  images  are converted into gray scale images so that they can be handled easily and require less storage.
The following equation shows how images are converted into gray scale images.
I(x,y)=0.2989*B +0.5870*G +0.1140*B
 
 
> Image Filtering
The PSNR value is calculated for  both the average and median resulting images .The average filter provides better result as compared to the median filter. So this paper uses average filter for further processing.
> Image Segmentation
To detect the pests from the images, the image background  is calculated  using  morphological operators which is most critical after this image is  subtracted  from  the original  image.  So  the resulting image will only have the objects with pixel  values  1 and  background pixel  values  0.
 
 
>Noise Removal
Noise contains dew drops, dust and other visible parts of leaves. As only the object of interest was to be visible on the images,so the aim was to remove the noise to get better and effective results. The Erosion algorithm has been used to remove isolated noisy pixels and to smoothen object boundaries . After noise removal,the next goal was to enhance the detected pests after segmentation which was performed by using the dilation algorithm.
>Feature Extraction
Different properties of the images are calculated on the basis of those attributes using which image is classified.  For image  properties, gray level co-occurrence matrix and regional properties  of the  images are  calculated. These properties  are used  to train the  support vector machine to classify images.
>Counting of the pests on the leaves is the main purpose, so that it can give an idea of how much pests are there on a leaf.It uses Moore neighborhood tracing algorithm and Jacob's stopping criterion
 
 Feasibility:
 
The present framework of pest detection is quite tedious and laborious for the farmers as they have to carry out their acre-acres surveys themselves and it requires a lot of vigorous efforts to achieve the same.Image analysis provides a realistic opportunity for the automation of insect pest detection.Through this system, crop technicians can easily count the pests from the collected specimens, and right pests’ management can be applied to increase both the quantity and quality of  production. Using the automated system, crop technicians can make the monitoring process easier.
So in order to bring enhancements in the system,we came up with more productive and well organised system with our idea .Due to this automaton applied,lucrativeness increases and labour is reduced.
