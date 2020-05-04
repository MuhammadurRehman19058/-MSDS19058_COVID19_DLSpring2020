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

![](Images/t1_v_t1_l.png)
![](Images/t1_v_t1_v.png)


![](Images/t1_r_t1_l.png)
![](Images/t1_r_t1_v.png)

Training, validatioin, Testing confusion Matrices
![](Images/t1_t1_v_c.PNG)
![](Images/t1_t1_r_c.PNG)

Task 2

![](Images/t1_v_t2_l.png)
![](Images/t1_v_t2_v.png)


![](Images/t1_r_t2_l.png)
![](Images/t1_r_t2_v.png)

Training, validatioin, Testing confusion Matrices
![](Images/t1_t2_v_c.PNG)
![](Images/t1_t2_r_c.PNG)

Task 3


![](Images/t1_v_t3_l.png)
![](Images/t1_v_t3_v.png)


![](Images/t1_r_t3_l.png)
![](Images/t1_r_t3_v.png)

Training, validatioin, Testing confusion Matrices
![](Images/t1_t3_v_c.PNG)
![](Images/t1_t3_r_c.PNG)

Test Accuracy Validation Accuracy, F1
![](Images/t1_v_chart.PNG)
![](Images/t1_r_chart.PNG)


For Epoch =10

![](Images/task%201-%20VGG16.PNG)
![](Images/task%201-%20resnet18.PNG)






__Task 2:__
In task w we were required to freeze some and freeze none layer the layers of conv layers and replace pre-trained model FC layers with our designed FC layers. Multiple tests have been performed by varying their learning rate, batch size and the results are as follows:


The loss and accuracy curve for Resent18 Entire model training are as follow

For Epcoch = 5

Task 1
![](Images/t2_v_t1_l.png)
![](Images/t2_v_t1_v.png)

![](Images/t2_r_t1_l.png)
![](Images/t2_r_t1_v.png)

Training, validatioin, Testing confusion Matrices
![](Images/t2_t1_v_c.PNG)
![](Images/t2_t1_r_c.PNG)


Task 2
![](Images/t2_v_t2_l.png)
![](Images/t2_v_t2_v.png)

![](Images/t2_r_t2_l.png)
![](Images/t2_r_t2_v.png)

Training, validatioin, Testing confusion Matrices
![](Images/t2_t2_v_c.PNG)
![](Images/t2_t2_r_c.PNG)


Task 3
![](Images/t2_v_t3_l.png)
![](Images/t2_v_t3_v.png)

![](Images/t2_r_t3_l.png)
![](Images/t2_r_t3_v.png)

Training, validatioin, Testing confusion Matrices
![](Images/t2_t3_v_c.PNG)
![](Images/t2_t3_r_c.PNG)



Test Accuracy Validation Accuracy, F1
![](Images/t2_v_chart.PNG)
![](Images/task2_resnet18_chart_e5.PNG)


For Epoch =10


![](Images/task%202-%20vgg16.PNG)
![](Images/task%202%20-%20resnet18.PNG)

![](Images/task2_rest18_entire_loss.png) 
![](Images/task2_rest_entire_accuracy.png) 


Please find the trained model of these assgienment on this link __Weights__ [link](https://drive.google.com/drive/folders/1bm45h4AL1S0H5-w_cLYkVQ8YPoWYD1VO?usp=sharing)







__PART 2__

For this part of the assignment we were supposed to train our VGG16 and Resnet 18 models for Multilabel Classification. We had to do mulitple experiments for Vgg16 and Resnet18 using BCEWithLogitsLoss and Focal Loss functions. Different experiments were performed by varing learning rate, batch size, epochs etc and Vgg16 performed outclass with highest training Accuracy(97.53%) and validation Accuracy(95.97%).


![](Images/b_v_t3_training_confusion.PNG)

![](Images/b_v_t3_validation_matrix.PNG)

![](Images/b_v_t3_loss.png)

![](Images/b_v_t3_accuracy.png)


You can find the data [here](https://drive.google.com/file/d/1eytbwaLQBv12psV8I-aMkIli9N3bf8nO/view?usp=sharing)


Please find the Trained [Weights](https://drive.google.com/drive/folders/1uqHNmW48Pu7MbM7Yg2xsddOjy_I6ZT66?usp=sharing)
