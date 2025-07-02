# 2025-WRO-Future-Engineering-LCDMC

## Contents

- [Preface](#Preface)
- [Design plan](#Design-plan)
- [Materials List](#Materials-List)
- [Photo](#Photo)
- [Videos](#Videos)


## Preface

We are from TWGHs Lee Ching Dea Memorial College.Our participants include Tsoi Ka Fu,Chong Ching Kit and Zhang Yuchao.This is our technical document.
Our team is made up of a group of student who love technology and robots.We hope to think about how robots can solve problems through innovative design,technology and different ideas,and in the upcoming WRO competition WRO competition,we will show our creativity,technology and strive for good results.

Therefore,in the WRO competiton.Our main goal is to show our problems-solving ability and teamwork.We hope to design and develop a robot that can solve practical problems.Therefore,we believe that only by constantly challenging ourselves can we achieve higher goals.Every competition is an opportunity to learn,and we will make full use of these experiences to make continuous progress and pursue excellence.

## Design plan

Regarding this WRO car, we use a custom car. It is rear-wheel-drive (RWD) to ensure its power supply. In addition, this car has a double-layer design. The bottom layer can hold different controllers such as batteries, motors and servos. On the second layer, we put orin nano 8GB to control the speed and direction of the vehicle. With this double-layer design, we put heavier objects on the lower layer, so the center of gravity of this car is low and it is not easy to tilt during operation.

### Obstacle Avoidance System Design
First,we take a set data of 'red' and 'green' blocks and label them through LabelImg.
![image](https://github.com/user-attachments/assets/39168842-af6d-4433-a47f-b599f73f51fa)
After that we build a model of yolo to tell Orin Nneo what the object is and it can give action

In code,we make use of yolo model to identify object with different colour and follow the flow show in figure1.1
![WhatsApp 图像2025-07-02于14 29 01_3eb417db](https://github.com/user-attachments/assets/583e9504-cbab-40c0-8966-1f92a848adce)
The code we accomplish this function are provided at 'code' 

### Velosity Controling System Design
At first,we set a throttle value at Orin Neno.We use a separate circuit board to run the PID programme to control and stablize the speed of car to allow us to stop the car at sutible palce on the track through counting the starting time

Here is the graphic shown of how each part of PID avoid the stablize of speed of car
![PID_Compensation_Animated](https://github.com/user-attachments/assets/0fff1022-56bb-44ba-ae9f-740df99037f7)

### Turning system design
We make use of road following model building method of jetson neno.

At first,we taking some image(around200) and use the different X coordinates repercent the turning (small x-coordinate mean turn left and large x-coordinate mean turn right)
![WhatsApp 图像2025-07-02于16 13 12_3bd753ba](https://github.com/user-attachments/assets/b7b7f950-68ac-4f28-852c-f695385f53c6)


## Materials List

- custom built car
- rear wheel drive wheel base
- metal gear servo
- 10A mosfet motor driver
- 7.4V 5200mah 25C Bettery
- 3D printed mounting board
- orin nano 8GB

## Team Photo
![IMG_20250702_155817](https://github.com/user-attachments/assets/6bad701f-2c3c-434e-b6f0-d1e99728f950)
![IMG_20250702_155833](https://github.com/user-attachments/assets/3525c81c-2976-4c74-8a9b-1a758f7c8962)



## Car Photo
![IMG-20250630-WA0079](https://github.com/user-attachments/assets/d156aeac-5f26-4984-ae09-9fdaf8254ea7)
![IMG-20250630-WA0078](https://github.com/user-attachments/assets/5be0584c-5c92-437a-9bd4-5d236d986abd)
![IMG-20250630-WA0077](https://github.com/user-attachments/assets/f4658fae-a32a-45c8-a2af-3caebeb7bcb7)
![IMG-20250630-WA0076](https://github.com/user-attachments/assets/eacca38f-a581-49d1-891c-a3d3c2c0d3ce)
![IMG-20250630-WA0075](https://github.com/user-attachments/assets/4aa4ae82-1c0e-480d-8446-e8f5ce290806)
![IMG-20250630-WA0074](https://github.com/user-attachments/assets/9ef45be5-e9cd-4fd0-8c68-6f31bf0c1be3)
![IMG-20250630-WA0073](https://github.com/user-attachments/assets/08a44a42-3eaa-490f-8d23-80814369ad71)
![IMG-20250630-WA0072](https://github.com/user-attachments/assets/621e8203-91a1-41d1-8fab-7b324057888d)
![IMG-20250630-WA0070](https://github.com/user-attachments/assets/476e0017-dec7-4be4-8b5f-56e16c0e99b6)
![IMG-20250630-WA0069](https://github.com/user-attachments/assets/45017fed-59e6-4d9e-a2be-5e160ccebc04)
![IMG-20250630-WA0082](https://github.com/user-attachments/assets/40623164-6cd5-441d-b2a8-21f8c94ee627)

## Videos

## Reference link
[1] https://github.com/HumanSignal/labelImg labelImg form Isell
[2]由 Physicsch - 自己的作品, CC0, https://commons.wikimedia.org/w/index.php?curid=40528698
