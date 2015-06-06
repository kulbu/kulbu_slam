# Kulbu

https://github.com/kulbu/kulbu/

# Kulbu SLAM

* Mostly launch files, some source testing tweaks here or there.
* Primarily focused on RTABMap.
* Turn camera 90deg for translational movement with LSDSlam.
* ORBSlam `config/orb/vocab.yml` excluded by `.gitignore`.

## Usage

```
roslaunch kulbu_slam rtab.launch
rosrun rviz rviz -d `rospack find kulbu_slam`/config/nav.rviz
roslaunch kulbu_slam rtabmapviz.launch
roslaunch kulbu_slam ratslam.launch
roslaunch kulbu_slam orb_slam.launch
rosrun lsd_slam_viewer viewer && rosrun lsd_slam_core live_slam image:=/stereo_camera/left/image_raw camera_io:=/stereo_camera/left/camera_info
```
