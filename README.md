# Where_am_I

This Project/zip file is of "Robot Localization". Since certain files are of large size, uploading to git was challenging even with 'Git LFS' henceforth a zip file. 

## Build and Run
* Download and extract the files to appropriate folder.
* Build the project
* Run 'world.launch' which also includes rviz_config and 'amcl.launch' files. 
* Ignore the initial warnings and wait roughly 10 seconds to upload 'map' in rviz 
* Use Nav-goal to set a destination/goal to robot. 

### Terminal 
```
git clone git@github.com:HarshaPhaneendra/Where_am_I.git
unzip Where_am_I.zip
mv -v Where_am_I/src/* /home/<username>/catkin_ws/src/
rm -rf Where_am_I
cd /home/<username>/catkin_ws
catkin_make
source devel/setup.bash
roslaunch my_robot world.launch

```

