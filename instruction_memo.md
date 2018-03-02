
# Submission

Udacity engineers will be evaluating your project on Carla, 
an autonomous Lincoln MKZ, at their test site in Palo Alto, California. 

The project that is evaluated on the vehicle should not have any external libraries
that aren't included in the starter repo.

Your team should be aware of the hardware specifications of the Udacity vehicle when designing your solution.


# Group formation

For this project you may work in groups of up to 5 students! 
If you would like to serve as the Team Lead for a group, 
add your name in the Team Lead section of the sign up sheet here. 
    https://docs.google.com/spreadsheets/d/17I_0q8tylk9Q_Y3GTSq738KkBIoS6SUt1quR5lPPAdg/edit?usp=sharing

Otherwise, find a team with additional space and add your name as a team member. 
Please sign up using the correct tab for your cohort. 

  Note that we'd like a minimum team size of 4, 
  so if you find that your team is not large enough, 
  you can merge with another team on the spreadsheet.

Udacity will be relativley hands-off in the team formation process, 
so you are welcome to structure the team and divide the work as you see fit. 
Feel free to create a private Slack channel for your team, 
set up meeting times, contribute to a shared repo, or more! 
If you are not already a member of the enrolled student Slack (different from ND013), you can join here.


2018/02/27

- Team Gauss
- Leader Sascha Moecker
  - mckeck88@gmx.de @sascha	UTC+1(Munich, Germany)
  - Used ROS in academia/industry
  - Happy with 4 teammates, contact using slack, starting on project start of March
- Team Member
  - Hiroshi Ichiki ichy@somof.net @hiroshi UTC+9 (Tokyo)
  - Saina Ramyar saina.ramyar@gmail.com	@saina UTC-5 (New York City)
  - David Obando david.obando@gmail.com	@davidobando UTC-8 (Seattle)
  - William Leu	reavenk@gmail.com @reavenk UTC-6 (Houston)



# Submission checklist and requirements

Once your team's project is able to drive the vehicle successfully in the simulator, 
you may be ready to submit the project for testing on the Udacity vehicle. 
At this point, your project should:

- Smoothly follow waypoints in the simulator.
- Respect the target top speed set for the waypoints' twist.twist.linear.x in waypoint_loader.py. 
  Be sure to check that this is working by testing with different values for kph velocity parameter
  in /ros/src/waypoint_loader/launch/waypoint_loader.launch. 
  If your vehicle adheres to the kph target top speed set here, then you have satisfied this requirement.
- Stop at traffic lights when needed.
- Stop and restart PID controllers depending on the state of /vehicle/dbw_enabled.
- Publish throttle, steering, and brake commands at 50hz.
- Launch correctly using the launch files provided in the capstone repo. 
  Please note that we will not be able to accomodate special launch instructions 
  or run additional scripts from your submission to download files. 
  The launch/styx.launch and launch/site.launch files will be used to test code in the simulator
  and on the vehicle respectively. 
  The submission size limit for this project has been increased to 2GB.

Udacity Self-Driving Car Harware Specs
- 31.4 GiB Memory
- Intel Core i7-6700K CPU @ 4 GHz x 8
- TITAN X Graphics
- 64-bit OS


# Project submission instructions

Once your project satisfies the conditions above, 
please follow these instructions to submit the project. 
Note that we will require a submission from each student in order to graduate. 

To prevent identical team member code from being run on Carla, 
there are different submission instructions for Team Leads and Team Members. 
We will run code and provide feedback for Team Lead submissions.



# simulator

mac_sys_int.zip

To improve performance while using a VM, 
we recommend downloading the simulator for your host operating system and using this outside of the VM. 

You will be able to run project code within the VM while running the simulator natively in the host using port forwarding on port 4567. 

uWebSocketIO Starter Guide
https://classroom.udacity.com/nanodegrees/nd013/parts/40f38239-66b6-46ec-ae68-03afd8a601c8/modules/0949fca6-b379-42af-a919-ee50aa304e6a/lessons/f758c44c-5e40-4e01-93b5-1a82aa4e044f/concepts/16cf4a78-4fc7-49e1-8621-3450ca938b77

For more information on how to set up port forwarding, see the end of the classroom concept here.



# Developping Environment

## ○Virtualbox
Udacity_VM_Base

## Ubuntu Native (unsupported)
Ubuntu 16.04
ROS
install

## Docker (unsupported)




