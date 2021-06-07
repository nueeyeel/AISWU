# AISWU

### **StyleGAN2 Detection**

___
A Study on the Characteristics of Stylegn2 Images to Find Optimal Detection Techniques
Lee yeeun, Yun Gyungeun, You haeun.

paper : https://stylegan2detect-aiswu.netlify.app

With the development of GAN (Generative Advanced Network), high-quality and high-resolution images can be generated. StyleGAN2 is a form of GAN that creates faces that do not exist. In this paper, StyleGAN2's facial image was detected from various perspectives. The eyes, nose, mouth and face were separated from the face image to learn the model, and the characteristics of StyleGAN2 were well reflected in which part of the face.

### **How to use**
>Only one image is possible. If you change the code, you can check many pictures.

test_img=" Put the image address you want to test in  "

test_mouth_img=" Enter the address of the location where the mouth will be stored "
test_nose_img=" Enter the address of the location where the nose will be stored "
test_eyes_img=" Enter the address of the location where the eye will be stored "
test_face_img=" Enter the address of the location where the face will be stored "

And then, at the end of the day, you'll see if this picture is 'real' or 'fake' (an image created with StyleGAN2)
Check to see if it is.

___

### **How to create**
>It trained StyleGAN2 photography with datasets of various nationalities, ages and genders. After setting the model and parameters properly, the model was trained.

### **About Dataset**

Images used for training provided here.

> FFHQ  : https://github.com/NVlabs/stylegan2

> Stylegna2-ADA : https://github.com/NVlabs/stylegan2-ada-pytorch

The image size of facial images generated by the StyleGAN2 model trained with datasets is 1024 x 1024. 1,500 images were collected equally among white, black, and Asian races and gender ratios.
<img width="904" alt="image" src="https://user-images.githubusercontent.com/41603416/121043026-3a0d6680-c7ef-11eb-9add-ef9903e6e1ed.png">

All data sets consist of high-quality images facing forward. The face was cut off from the image using dlib, and the eyes, nose, and mouth were cut off from the face area using mtcnn. XceptionNet and Inception-ResNet-v2 are used to learn the cut-off image, and high-precision models are used to make comprehensive judgments.

___

### **F-1 score and Accuracy for images by face area**
Performance evaluation was conducted using 1,000 high-quality real images and 1,000 StyleGAN2-ffhq images that do not overlap with the training dataset. The real image used in the test was selected as a dataset similar to the image quality used in the training.

>real image used in the test :  https://www.kaggle.com/ciplab/real-and-fake-face-detection

<img width="809" alt="image" src="https://user-images.githubusercontent.com/41603416/121050903-f23d0e00-c7f3-11eb-9e96-efdc3850a88d.png">


### **How to contact us**
>aiswuproject@gmail.com 
