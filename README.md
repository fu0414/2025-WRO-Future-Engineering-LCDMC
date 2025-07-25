# 2025-WRO-Future-Engineering-LCDMC

## Contents

- [Preface](#Preface)

- [Design plan](#Design-plan)

  -[Obstacle Avoidance System Design](#Obstacle-Avoidance-System-Design)
  
  -[Velosity Controling System Design](#Velosity-Controling-System-Design)
  
  -[Turning System Design](#Turning-System-Design)
  
- [Materials List](#Materials-List)

- [Team Photo](#Team-Photo)

- [Videos](#Videos)

  -[Anti-clockwise non-obstacle track](#Anti-clockwise-non-obstacle-track)
  
  -[Anti-clockwise obstacle track](#Anti-clockwise-obstacle-track)
  
- [Reference link](#Reference-link)


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
![WhatsApp 图像2025-07-02于18 45 39_e29862a7](https://github.com/user-attachments/assets/c8c6baf2-1c4a-4e26-bd1d-637abf77bf8b)
The code we accomplish this function are provided at 'code' 

### Velosity Controling System Design
At first,we set a throttle value at Orin Neno.We use a separate circuit board to run the PID programme to control and stablize the speed of car to allow us to stop the car at sutible palce on the track through counting the starting time

Here is the graphic shown of how each part of PID avoid the stablize of speed of car
![PID_Compensation_Animated](https://github.com/user-attachments/assets/0fff1022-56bb-44ba-ae9f-740df99037f7)

### Turning System Design
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

## Videos
### Anti-clockwise non-obstacle track
https://youtu.be/owy3CJZng4w?si=nF-QKbm0MD8-GtaB

### Anti-clockwise obstacle track
https://youtu.be/lJq19d5X1js?si=-KF2ZG_xXKJI6lv7


## Reference link
[1] https://github.com/HumanSignal/labelImg labelImg form Isell

[2]由 Physicsch - 自己的作品, CC0, https://commons.wikimedia.org/w/index.php?curid=40528698
