# DatasetVisualization
This architecture will allow user to visualize the content of Dataset created by our team members.

## Authors
* ZAID : zaidrafi107@gmail.com

## Architecture of the System
Datavisualization GUI is the overall graphical part of the visualization system where user can examine Rosbags i -e The already built dataset of three sensors (Kinect, SmartWatch,  Motion Capture Sensor MOCAP) with their respective datatypes (PointCloud2, IMU, Float32). The GUI enable the user regarding the managing the configuration of Rosbags, let the user to keep the track of time through a timer and the executed percentage of the bag files via Progressbar. GUI consist of three borwising options for the respective sensors, which allows the user to navigates through the system to a folder that contains the required bag files. Upon selecting, the path address will be displayed for an added certainty. After loading the bag files to the GUI, "PlayAll" button will initiate the Processing of the files by keeping track of them via Timer, ProgressBar and a slider. Below each of the display window there is STOP button which also works in individual capacity, while StopAll button will bring the system to reset. 
 
![Archietecture](https://user-images.githubusercontent.com/63880770/96398805-07195280-11cd-11eb-98fe-a4c83a922050.png)



## Contents of the repository
In this section we will explain the repository's content.

### GUI Pictures
Pictures of the visualization window are shown here for user to have a clear idea of how the GUI looks

### Documentation
This directory contains the doxygen documentation in "html" and "latex" format. For a clear and better idea of the project script and its detailed explanation, go to 

```
documentation/index/index.html
```

### Src
This folder contains a python script for the initialization of the MainwWindow. It also contains a file by the name of "final.ui" which is GUI created in Qt designer. For execution of the python script, both the python script and Qt designer file should be in the same directory. There are two other files, resource file with extension ".qrc" and a picture. Both of them are important part of the GUI created in qt designer and the GUI cant be initialized without these two files in the same directory.

## Installation
The first thing to do, after having cloned the repository in the Ros workspace, is to build the package and install in order to make the files executable, using the following commands in the workspace:
    
    ```
    catkin_make
    catkin_make install
    ```

Execute the following commands for Ros related Python libraries 
    
    ```
	sudo apt-update
	sudo apt install python3-pip
    sudo apt-get install python3-yaml	
    sudo pip3 install rospkg catkin-pkg 
    pip3 install --user pyqt5
	sudo apt-get install python3-pyqt5
    ```


## Work In Progress
The existing GUI is just a model and doesnt visualize anything in real. Other members of the team are working on the real time visualization of the bag files. Fow now,this GUI just contains a widget box while rest of the above described architecture works perfectly.

