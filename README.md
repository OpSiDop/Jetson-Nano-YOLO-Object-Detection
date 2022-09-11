# Object-Detection-in-Jetson-Nano
# NVIDIA Jetson Nano 
![jetson](https://user-images.githubusercontent.com/75358720/189518011-1d189aaf-bfdf-4d54-b41b-495afd89cf15.jpg)


The NVIDIA Jetson Nano Developer Kit is an AI computer for makers, learners, and developers that brings the power of modern artificial intelligence to a low-power, easy-to-use platform. Get started quickly with out-of-the-box support for many popular peripherals, add-ons, and ready-to-use projects. 

We are grateful to NVIDIA and SRM Institute of Science and Technology for giving us the opportunity to work on this project.

# Setting up NVIDIA Jetson Nano
For setting up the kit for the first time we reffered to the tutorial made by the NVIDIA Developer - [Vedio Link](https://youtu.be/uvU8AXY1170)


Other than the kit we have connected some other required objects-
1. IMX-219-77 Camera Module 
2. Ethernet connection
3. External Monitor/Display
4. 32GB MicroSD Card
5. HDMI Cable
6. Power Adapter with Supply
![image](https://user-images.githubusercontent.com/93781577/189525144-123a5efe-793d-4be1-82c5-d4fcef20266c.png)

# Setting up YOLO-Object Detection
1. We will be installing Darknet using the Jetson's terminal from [AlexeyAB/darknet](https://github.com/AlexeyAB/darknet.git).
 ```
 git clone https://github.com/AlexeyAB/darknet.git
 cd darknet
 ```
 
2. Enable GPU and OpenCV support by editing the Makefile and also compile the makefile-
 ```
 sudo nano Makefile
 ```
   Set the following values to enable GPU and OpenCV support-
 >  GPU=1
 
 >  CUDNN=1
 
 >  OPENCV=1

 ```
 make
 ```

3. To run object detection with Darknet, we need a model config and model weights(in the cfg directory).
 ```
 wget https://pjreddie.com/media/files/yolov3.weights
 wget https://pjreddie.com/media/files/yolov3-tiny.weights
 ```

4. We are done with installation part and we need to run the camera module to see the predictions in real time-
 ```
 detectnet-camera.py
 ```


# Results from our kit -
https://user-images.githubusercontent.com/93781577/189527141-5a412f5c-7793-498a-8708-5013a0a5fde1.mp4

## Authors  -
<div align="left"> 
  <table>
<tr align="left">
 <td>

####     Aryan Raj
<p align="center">
<img src = "https://avatars.githubusercontent.com/u/75358720?v=4"  height="120" alt="Aryan Raj">
</p>
<p align="center">
<a href = "https://github.com/aryanraj2713"><img src = "http://www.iconninja.com/files/241/825/211/round-collaboration-social-github-code-circle-network-icon.svg" width="36" height = "36"/></a>
<a href = "[https://www.linkedin.com/in/aryan-raj-3a68b39a/](https://www.instagram.com/aryan_raj_1312/)">
<img src = "[http://www.iconninja.com/files/863/607/751/network-linkedin-social-connection-circular-circle-media-icon.svg](https://www.iconninja.com/files/268/699/635/instagram-icon.png)" width="36" height="36"/>
</a>
</p>
 <strong>ML and CV Developer<strong>
</td>


 <td>

####  Sidhartha Raghaw
<p align="center">
<img src = "https://instagram.fmaa8-1.fna.fbcdn.net/v/t51.2885-15/273433026_102563928955254_1782636919767645604_n.webp?stp=dst-jpg_e35&_nc_ht=instagram.fmaa8-1.fna.fbcdn.net&_nc_cat=106&_nc_ohc=NXTVNl28yy4AX_OnZMS&edm=ALQROFkBAAAA&ccb=7-5&ig_cache_key=Mjc2ODU0NzE5MzMxMTY0ODkyMA%3D%3D.2-ccb7-5&oh=00_AT9oiwIVRFLnJvGc2BfW9flk8DQv28zHYNyzU2KSFn2E8w&oe=63254BB9&_nc_sid=30a2ef"  height="120">
</p>
<p align="center">
<a href = https://github.com/OpSiDop"><img src = "http://www.iconninja.com/files/241/825/211/round-collaboration-social-github-code-circle-network-icon.svg" width="36" height = "36"/></a>
<a href = "https://www.instagram.com/pssy_destroyer_sid/">
<img src = "[http://www.iconninja.com/files/863/607/751/network-linkedin-social-connection-circular-circle-media-icon.svg](https://www.iconninja.com/files/268/699/635/instagram-icon.png)" width="36" height="36"/>
</a>
</p>
 <strong>FLUTTER Developer<strong>


   

 <td>

####        Paras Atal
<p align="center">
<img src = "https://instagram.fmaa8-1.fna.fbcdn.net/v/t51.2885-15/296315596_190398770048024_3637669814111720342_n.webp?stp=dst-jpg_e35&_nc_ht=instagram.fmaa8-1.fna.fbcdn.net&_nc_cat=108&_nc_ohc=RlcfJ6xf54cAX9l6dFc&edm=ALQROFkBAAAA&ccb=7-5&ig_cache_key=Mjg5MzgzMTE0NDQ5NTk3NjcwMQ%3D%3D.2-ccb7-5&oh=00_AT_u9TsDtmoWTxVNfGSZQiIA_fLC7442wbt5fFttMm8Wqg&oe=632412DD&_nc_sid=30a2ef"  height="120" >
</p>
<p align="center">
<a href = "https://github.com/ParasAtal"><img src = "http://www.iconninja.com/files/241/825/211/round-collaboration-social-github-code-circle-network-icon.svg" width="36" height = "36"/></a>
<a href = "[https://www.linkedin.com/in/nikhil-ivannan-351036201/](https://www.instagram.com/paras_atal/)">
<img src = "https://www.iconninja.com/files/268/699/635/instagram-icon.png" width="36" height="36"/>
</a>
</p>
 <strong>Competitve Programmer<strong>
</td>
  <td>
