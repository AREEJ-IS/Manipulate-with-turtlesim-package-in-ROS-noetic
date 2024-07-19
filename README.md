# Manipulate-with-turtlesim-package-in-ROS-noetic

After installing and setting up ROS, we will go through the steps of manipulating the turtle package in ROS-noetic

First, we will open a terminal and it is important to start the ROS master node using the command:
```
roscore
```
<img width="960" alt="التقاط PNG-" src="https://github.com/user-attachments/assets/5f617f85-7b1a-49ff-82a7-75d7634b8bc6">

I opened another terminal. I will try running ros master again to see what happens 

<img width="958" alt="k" src="https://github.com/user-attachments/assets/ebcd848d-aeab-4efe-86a0-4dac936d70cb">

Notice that I get an error when I run ros master again ، The reason for this error is that we already have a ros master that works well, so if you want to start a ros master program, you can only get one.

## manipulate with some packages

When we install ros, we already have nodes that you can start, you have typical nodes for educational nodes and several nodes for different functions.
#### 1-so to start a node we will use the command which looks like a program that will print "hello World" into the terminal with a timestamp

```
rosrun rospy_tutorials talker
```
<img width="473" alt="u" src="https://github.com/user-attachments/assets/8a18b11a-0f7d-429b-8365-c58902bb2bd0">

if you want to stop the node you can press (ctrl + C)
But so that you do not see an error or deficiency, do not stop it

#### 2-Open another terminal and type this command which allows you to get a graphical view of the actual ROS (nodes, topics and connections running on your computer)

```
rqt_graph
```
<img width="468" alt="ii" src="https://github.com/user-attachments/assets/45183e20-b0ab-437d-af2c-d45841f53c95">

you can see that here we have ONE node named (talker)

#### 3- this is another program that is going to print something in the terminal, and (heard) hello world with the timestamp. actually this data coming from the (talker) node

<img width="960" alt="e" src="https://github.com/user-attachments/assets/3508a8a9-7fee-4a1e-bcfe-4c33e607a160">

You can see that here we have a token node. Here we have a (listener) node and we also have a (talker) node. The talker node sends some things to the listener node.


## Turtlesim
1- This command is going to show a graphical window with a turtle
```
rosrun turtlesim turtlesim_node
```
<img width="472" alt="o" src="https://github.com/user-attachments/assets/6d3e6a3b-c8d8-4005-a303-4939ed4e771b">

2- this command will allows you to control the turtle with aarrow keys of your keyboard
```
rosrun turtlesim turtle_teleop_key
```
<img width="666" alt="ll" src="https://github.com/user-attachments/assets/eacb4ca1-9a38-4a27-920c-fbeeadf5dddd">

note: if the turtle does not moving, make sure to click the terminal window that contains (rosrun turtlesim turtle_teleop_key) command.
