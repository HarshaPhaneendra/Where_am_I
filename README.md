# Where_am_I

This Project is of "Robot Localization". Since certain files are off larger size, uploading to git was challenging even with 'Git LFS' henceforth a zip file.

## Build and Run
* Download and extract the files to appropriate folder.
### Terminal 1
```
git clone git@github.com:HarshaPhaneendra/Where_am_I.git
unzip Where_am_I.zip
mv -v Where_am_I/src/* /home/<username>/catkin_ws/src/
rm -rf Where_am_I
```
* Build the project
```
cd /home/<username>/catkin_ws
catkin_make
source devel/setup.bash
```
* Run 'world.launch' which also includes rviz_config and 'amcl.launch' files. 
* Ignore the initial warnings and wait roughly about 10-15 seconds to upload 'map' in rviz.
* Use Nav-goal to set a destination/goal to robot. 
```
roslaunch my_robot world.launch
```
* Alternative way to use "teleop_twist_keyboard" pkg. 
* Use keyboard to move robot.
### Terminal 2
```
cd /home/<username>/catkin_ws
source devel/setup.bash
rosrun teleop_twist_keyboard teleop_twist_keyboard.py
```
