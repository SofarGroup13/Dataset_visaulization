# DatasetVisualization
This architecture will allow user to visualize the content of Dataset created by our team members.

## Authors
* ZAID : zaidrafi107@gmail.com

## Architecture of the System
Datavisualization GUI is the overall graphical part of the visualization system where user can examine Rosbags i -e The already built dataset of three sensors (Kinect, SmartWatch,  Motion Capture Sensor MOCAP) with their respective datatypes (PointCloud2, IMU, Float32). The GUI enable the user regarding the managing the configuration of Rosbags, let the user to keep the track of time through a timer and the executed percentage of the bag files via Progressbar. GUI consist of three borwising options for the respective sensors, which allows the user to navigates through the system to a folder that contains the required bag files. Upon selecting, the path address will be displayed for an added certainty. After loading the bag files to the GUI, "PlayAll" button will initiate the Processing of the files by keeping track of them via Timer, ProgressBar and a slider. Below each of the display window there is STOP button which also works in individual capacity, while StopAll button will bring the system to reset. 
 
![Archietecture](https://user-images.githubusercontent.com/63880770/96398805-07195280-11cd-11eb-98fe-a4c83a922050.png)


## Work In Progress
The existing GUI is just a model and doesnt visualize anything in real. Other members of the team are working on the real time visualization of the bag files. Fow now,this GUI just contains a widget box while rest of the above described architecture works perfectly.
