Launch simulation:

  source install/setup.bash
  
  
  ros2 launch test_bot launch_sim.launch.py world:=<path_world>   #Launch gazebo
  
  
  ros2 launch test_bot rviz_launch.launch.py use_sim_time:=true     #Launch rviz
  
  
  ros2 launch test_bot online_async_launch.py use_sim_time:=true  #Launch slam_toolbox to create a map
  
  
  ros2 launch test_bot localization_launch.py map:=<path_map> use_sim_time:=true #Launch localization if you already had a map
  
  
  ros2 launch test_bot navigation_launch.py use_sim_time:=true    #Launch nav2
   
   
   
BUG NEED TO FIX: 

  - When running slam_toolbox Nav2 will not response correctly 
  
  - Launch file localization can not get the map's path need to do manually
  
  - When localization map will not auto update need to do manually
  
  - When running real robot ros2_control: control_manager only get data from adruino hardware, need to add drive to work with another SoC 



  

