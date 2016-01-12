# bml\_vrep

Code for running vrep simulations of Biomimetic Millisystems Lab robots with ROS

Setup
=====

 * Install v-rep 3.2.2
 * Add environment variable VREP\_ROOT\_DIR to bashrc that points to v-rep isntall directory
 * Add VREP\_ROOT\_DIR to path
 * Create ROS workspace and add this repo, as well as a symbolic link to the full path to VREP\_ROOT\_DIR/programming/ros\_packages to the worspace src directory
 * Create a symbolic link to VREP\_ROOT\_DIR/programming/ros\_packages/ros\_bubble\_rob/include/v\_repConst.h in this repo's include directory
 * Create a symbolic link to VREP\_ROOT\_DIR/vrep.sh in this repo's src directory

Running Demo
============

 * roslaunch bml\_vrep demo.launch
 * (in a separate terminal for each robot, replace n with robot number) roslaunch bml\_vrep keyboard\_input.launch robot=robot\_n
 * To quit, find the keyboard input window (should have a keyboard icon in the taskbar) and enter q in it before ctrl-c killing everything else
