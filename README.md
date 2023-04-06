Launch simulation:

  #Always source first
    source install/setup.bash
  #Launch gazebo
    ros2 launch test_bot launch_sim.launch.py world:=<path_world>
  #Launch rviz
    ros2 launch test_bot rviz_launch.launch.py use_sim_time:=true   
  #Launch slam_toolbox to create a world
    ros2 launch test_bot online_async_launch.py use_sim_time:=true  
  #Launch localization if you already had a map
    ros2 launch test_bot localization_launch.py map:=<path_map> use_sim_time:=true 
  #Launch nav2
    ros2 launch test_bot navigation_launch.py use_sim_time:=true
   
   
TODO: 
  -When running slam_toolbox Nav2 will not response



  

