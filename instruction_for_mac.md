
To extract at the command line in macOS or Linux:

1. Open Terminal and navigate to directory containing the compressed image
3. execute $ unzip Udacity_VM_Base_V1.0.0.zip

In the zipped archive in addition to the VM disk image, there are two
other small configuration files that you may or may not need.

We recommend using VirtualBox to run the VM. This will enable you to easily use port forwarding, so you can run the final project simulator in your native operating system (the host) while using the VM for running ROS code.

Whichever operating system you're on, download and install the appropriate platform package for your operating system (the host) and then follow the instructions below:



Import your VM image to VirtualBox

- Download and install VirtualBox.
- Download the image from supplied link.
- Unzip the image.
- Open VirtualBox Application.
- Click File > Import Appliance..
- Click the folder icon on the right and navigate to your unzipped image (the .ovf file).
- Follow the prompts to import the image.
- From the VirtualBox Manager, select your VM and press start.


user: student
pass: udacity-nd



source /opt/ros/kinetic/setup.bash




Troubleshooting Tips

- Keyboard Mappings: Use of certain keyboards can create issues unless the corresponding keyboard has been set in the VM. This is due to keyboard mappings. A frequent issue is special characters in passwords not being entered correctly when logging in. An example useage for VirtualBox is setting up an Italian keyboard. To do this, execute the following in a terminal localectl set-keymap it; localectl set-x11-keymap it.

- roscore ip: If the host network interface has multiple addresses (ex: ipv6 enabled) roscore will fail since hostname -I returns multiple ip, resulting into a invalid URL. One solution to this is to replace this line in .bashrc, export ROS_IP=`echo $( hostname -I)' , with this export ROS_IP=$( hostname -I | awk '{print $1}').



Environment Setup

    source /opt/ros/kinetic/setup.bash



# Install Error

https://discussions.udacity.com/t/some-trouble-shootings-on-installing-ros-on-mac/530986



# DataSet

## Bosch Traffic Sign Database

https://hci.iwr.uni-heidelberg.de/node/6132

non commercial use only

Bosch Small Traffic Lights Dataset
https://github.com/bosch-ros-pkg/bstld


forum
https://discussions.udacity.com/t/do-we-need-to-develop-traffic-light-detector-or-is-it-supplied/411551/13

JacquesRoth Jan 13

My group experimented with the Bosch dataset and traffic light detection with machine learning. 
Did not get too good a result for Carla and the processing time seemed too long so we ended up using a machine vision approach with OpenCV. 
My own personal reservations were that both the simulator traffic lights and Carla lights were very non-standard. 
But others have suggested using this Bosch dataset and implied they had success. 
The interesting thing is the Bosch dataset worked better with the simulator than with Carla. 
Personally, for the simulator I would be tempted to train on images created by extracting and morphing traffic lights in the simulator frames.
