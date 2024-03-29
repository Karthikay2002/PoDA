# PoDA

# Inspiration:-

 We are in a time where the outcomes of poaching are given a lot of value and money even though it is 
considered illegal. Every day we are <b>losing hundreds of mammals belonging to endangered species</b> 
this is mainly due to the lack of enforcement and proper 
government regulations. The increased demand in boasting of pride in holding animal assets has crossed the limit, which made poachers, money-making entities in the black market. Continuous monitoring by the park rangers would be a tedious task and may not even be done properly at times too. Animal Poaching has become a global problem of the 21st century. The increased spike in the rate of animal poaching is miserable to know. A part of this can be approached by using cuttingedge technologies. The Internet of Things and Computer Intelligence are few technologies that have been stupendously emerging hand in hand and can be used to solve world pressing problems.

# Proposed Solution:-

The prototyped solution would have a life-changing impact on 
animals and probably help us catch the predators too. Implementing this 
technology solution into the real world,red uces the poaching curve to the 
minimum. Not only being the eyes from the sky, our prototype can get the clear 
image of the terra-firma and detect what is what with the help of its camera.

It flies down to a stealth level and sends us the interactive feedback of the place by taking a video or a photo.
This solution can detect people, weapons, animals, trees and many more. 
Further developments in this project include the predicting of the type animal and the exact location of the hunt, so that the task force could immediately come to the respective place and act.
The respective organizations need not require any strains and moreover it need not rely on other solutions by utilizing the product. The lives of animals will get  saved from <b>poaching</b>.

The prototype will change into an <b>“Aerial surveillance”</b> once it takes off to the heights of the skies/clouds once we market it and make it even more scalable. This is completely remote controlled (for now at least).

Using the latest advances in Machine Learning and Computer Vision, we are trying to transform the lives of the muted ones (animals).

<b>DRONEYES</b> can describe what’s going on the ground through the video output we get on the user side. It can help to find things around the scouted area by describing, which is human, animal (by species) immediately and gives the exact position of the area that needs to be scouted. With the help of cloud technology, we can share the data in real time. 

We are trying to integrate the object detection software into the drone’s camera which is a big challenge.

We are working on the GPS module and the Flight Controller for the drone. The flight controller is necessary for the stability of the drone. The Global Positioning System or GPS is a device that has a capability to measure how long a signal takes to travel from a satellite. This device gives an estimation of the drones altitude, the lat and the long of the place. This makes the device to be so vital in our project. The GPS modules are inaccurate, but they can be rectified by buying more complex external GPS receivers. For this project we are using Neo 6m v2 GPS Module, this module has a high precision output.This module comes pre-equiped with a battery due to which we can obtain the GPS lock faster. 
The antena is also connected to the module through the cable which allows for easy mounting of the GPS. This makes it to see the sky and give its best performance. When it comes to accuracy, we can expect an error upto 4 times the pixel size for a correctly reconstructed model.


We collected few videos from the sourceful web, and then we ran our software on the video and the results are pretty amusing. It went well. 
We took a video of a neighbourhood which has cars and trucks and another video from NatGeo Wild. One is for detecting the cars and the other is for detecting the types of animals.  Accompanying the current world technological advancements in the Internet Of Things and Deep Learning; Object detection has become an effortless job. The goal of our research is to achieve a feasible perspective on anti-poaching.
The software model we used is YOLOv3

# How we built it?
 
The prototype will change into an “Aerial surveillance” once it takes off to the heights of the skies/clouds once we market it and make it even more scalable. 
This is completely remote controlled (for now at least).
Using the latest advances in Machine Learning and Computer Vision, we are trying to transform the lives of the muted ones (animals).
DRONEYES can describe what’s going on the ground through the video output we get on the user side.
It can help to find things around the scouted area by describing, which is human, animal (by type) immediately and gives the exact position of the area that needs to be scouted.
With the help of cloud technology, we can share the data in real time.

# WORKFLOW

<img src="img/flowchart.jpeg">

1) Once the GPS location and the area has to be set
2) Animal or a Human has been detected by the Raspberry Pi Camera 
3) The object detection Algorithm start running
4) Alert is sent to the Base camp about what is seen by the camera from the detection
5) GPS and the pictures are sent as an alert
6) The above data is sent as an encrypted data, for not looksing it to cyber threat.
# Challenges we ran into:-

1)	Integrating the object detection into the drone’s camera is a big challenge that we faced during the hackathon.
2)	The drone’s flight controller gave us a trouble during the hackathon, this made us tensed and nervous about the result, but we finally made it possible by solving it.
3)	The most important thing is to integrate the sub-modules to a whole project prototype.

# Accomplishments we are proud of!
 We knew it was a hard task to implement our idea on a totally new platform and environment without our physical selves being at one place due to COVID-19, but we challenged ourselves to fight it till the end and we did it. Being able to transform our idea into a project that could be displayed feels great! We will never step back in life from trying something new every time. If we could stay up for 24 hours and accomplish our goal, we believe nothing is IMPOSSIBLE.
 
# Future Scopes
Making major advancements in the image overflow, making image enchancements to incerease the acurracy of the detection

The need to cover larger land/area in shorter time is demanding. This can be only done by launching a network of these low-cost UAV's- SWARM ROBOTICS

Shifting the Object Detection into the cloud by using AWS or AZURE cloud services would help to make the product more technical.

 Edge computing using high performance computers, like jetson nano is a future step. Securing and sharing the data to make it even more safe from threats



# OBJECT DETECTION

    1. Real Time
    2. Video Feed
    
<b>YOLOv3</b> trained on <b>COCO</b> was used for Object detection. Darkflow which is a Tensorflow variant Darknet was used to process the frames. Darknet is an open source neural network framework written in C and CUDA. 

<img src="https://github.com/yuvaraj-06/ETHEREUM-DRONEYES/blob/master/object%20detection/img/yol.jpg">


Several images of Guns, Poachers, Rangers were scraped from the internet and YOLOv2 was trained from scratch to detect the following object classes in the frames. Due to lack of data and time in the hackathon, high accuracy and confidence was not achieved.

Wildlife Video Feed was fed to the layers of YOLO and animals / humans were tracked with high confidence in the wildlife. Some of the frames are :

<img src="https://github.com/yuvaraj-06/ETHEREUM-DRONEYES/blob/master/object%20detection/img/xlmr.JPG">


# Steps For Using Object Detection

<b>STEP-1</b> Download the current repositry.

<b>STEP-2</b> Open command promt and cd to object detection .

<b>STEP-3</b> Then type <b>python webstreaming.py -i 127.0.0.1 -o 5000</b> .

<b>STEP-4</b> Then you can see , a self host server running and copy this link <b>http://127.0.0.1:5000/</b> and paste in browser.

<img src="https://github.com/yuvaraj-06/ETHEREUM-DRONEYES/blob/master/object%20detection/cmd.PNG">

# Steps For Running BlockChain Application


### Install dependencies:

```
cd blockchain
npm install
```
Run the server:

```
npm start
```


### Point the web browser at the demo:

```
http://localhost:3000
```
<img src="img/cmd.JPG">

# BLOCKCHAIN APPLICATION IMAGES

<img src="img/hash.JPG">
<img src="img/block.JPG">
<img src="img/chain.JPG">
<img src="img/work.JPG">

# DRONE IMAGES

<img src="img/WhatsApp Image 2020-06-21 at 2.50.56 PM.jpeg">

