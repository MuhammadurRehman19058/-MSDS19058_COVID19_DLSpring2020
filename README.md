# MSDS19058_COVID19_DLSpring2020

__Objective:__
In this assignment we were required to detect infections of Coronavirus using X-Rays images. To do so, we were supposed to
•	Use CNN, pretrained ImageNet, to extract basic features from X-Ray images
•	Train classification layers in order to detect instance of Infected and Normal X-Ray Images
•	Fine-tune the entire network to try to improve performance

__Dataset:__ [link](https://drive.google.com/drive/u/0/folders/1-FzZhQO9oHIT9SNOWYoKsuz7fe447vtR)

The dataset contains 2 classes “infected” and “normal” and their details are as follow:



![](Images/Dataset_details.PNG)

The X-Ray Images are taken in different vies (AP or PA) depending the side of the is facing the X-Ray scanner but we be using these images without considering their view. A few sample images:

![](Images/Xray_image.PNG)


__Task 1:__
In task 1 we were required to freeze all the layers except the FC layers and replace them with our designed Fc layers. Multiple tests have been performed by varying their learning rate, batch size and the results are as follows:

For Epoch = 5

Task 1

![](Images/t1_v_t1_l.PNG)
![](Images/t1_v_t1_v.PNG)


![](Images/t1_r_t1_l.PNG)
![](Images/t1_r_t1_v.PNG)

Task 2

![](Images/t1_v_t2_l.PNG)
![](Images/t1_v_t2_v.PNG)


![](Images/t1_r_t2_l.PNG)
![](Images/t1_r_t2_v.PNG)

Task 3

![](Images/t1_r_t3_l.PNG)
![](Images/t1_r_t3_v.PNG)


For Epoch =10

![](Images/task%201-%20VGG16.PNG)
![](Images/task%201-%20resnet18.PNG)



![](Images/task1_rest_FC_only_loss.PNG)
![](Images/task1_rest_FC_accuracy.PNG)



__Task 2:__
In task w we were required to freeze some and freeze none layer the layers of conv layers and replace pre-trained model FC layers with our designed FC layers. Multiple tests have been performed by varying their learning rate, batch size and the results are as follows:

![](Images/task%202-%20vgg16.PNG)
![](Images/task%202%20-%20resnet18.PNG)

The loss and accuracy curve for Resent18 Entire model training are as follow

For Epcoch = 5

Task 1
![](Images/t2_r_t1_l.PNG)
![](Images/t2_r_t1_v.PNG)

Task 2
![](Images/t2_r_t2_l.PNG)
![](Images/t2_r_t2_v.PNG)

Task 3
![](Images/t2_r_t3_l.PNG)
![](Images/t2_r_t3_v.PNG)

For Epoch =10

![](Images/task2_rest18_entire_loss.PNG) 
![](Images/task2_rest_entire_accuracy.PNG) 



