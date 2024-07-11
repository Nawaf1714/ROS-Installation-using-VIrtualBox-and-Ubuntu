# ROS-Installation-using-VIrtualBox-and-Ubuntu
The first task in the path of artificial intelligence

These instructions will install ROS Noetic Ninjemys, which is available for Ubuntu Focal (20.04), Debian.
## Links
VirtualBox
- https://www.virtualbox.org/wiki/Downloads

Ubuntu
- https://ubuntu.com/download/desktop

for help and more details 
- https://wiki.ros.org/noetic/Installation/Ubuntu

##

Install ROS noetic
Explanation of the steps

In the beginning, in order to be able to download the ROS, we need the Ubuntu system (which is Linux).

We will need a tool to run the Links system on our devices, which is VM VirtualBox..

This is the link to download VirtualBox:
( https://www.virtualbox.org/wiki/Downloads )

Then select the version for our device.

After the virtualbox is loaded, we go to download the Ubuntu system…

This is the link to download Ubuntu :
( https://ubuntu.com/download/desktop )
Then select the version 20.04

The link will be downloaded in (iso) format.


-  we start running the virtualbox and create a new system by clicking on ( new ) 
- After the system name is created, we place a link to download Ubuntu OS.
- set memory size (RAM)
- set size of virtual hard disk 

Then the basic settings for downloading and installing the new system.

## And the First of the steps of our basic mission:

install ROS 
open the ( TIRMINAL) and Write..

### 1.1 Setup your sources.list

     sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

### 1.2 Set up your keys

    sudo apt install curl # if you haven't already installed curl

    curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -

### 1.3 Installation 
First, make sure your Debian package index is up-to-date:
    
    sudo apt update

Desktop Install: Everything in ROS-Base plus tools like rqt and rviz (Recommended)

    sudo apt install ros-noetic-desktop

### 1.4 Environment setup  

You must source this script in every bash terminal you use ROS in.

    source /opt/ros/noetic/setup.bash

finally you can run The ROS command by typing : 

    roscore 



