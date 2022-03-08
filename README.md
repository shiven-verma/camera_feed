# Getting Camera Feed in ROS
This package includes a simple publisher and subscriber to get camera feed from your **primary camera** 
on your system and publish it on a topic. 

You should have **openCV** installed.we are going to use that in our code to capture video.

you can use command :  <code>$ rostpic echo ($TOPIC_NAME)</code> to see the message being published.

### How to use
 1. Clone the repo in your workspace directory: 
  ```
  $cd catkin_ws/src
  $git clone https://github.com/shiven-verma/camera_feed 
  ```
  
 2. Build the package
 
 ```
 $cd ..
 $catkin_make
 ```
 3. Now source the package and make files executable
 
  ```
  $source devel/setup.bash
  ```
  
  making files executable 
  
  ``` 
  chmod +x ($FILE_NAME)
  ```
 4. Now either we can publish our camera_feed on a topic and use any subscriber to get the feed 
  ```
   $ roslaunch publisher.launch
  ```
  or see the feed on screen 
  
      $ roslaunch show.launch 
      
      
      
  I will be using this repo for my openCV projects.
