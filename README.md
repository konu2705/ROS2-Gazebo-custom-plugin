# ROS2-Gazebo-custom-plugin

THIS WORKS!!! IT TOOK A LOT OF TIME TO FIND THE RIGHT THINGS TO MAKE IT WORK BE CAREFUL!!

Cmakelist file mai there is no need for executable comand when making a plugin


the following lines are the one which finally after a whole day of work allowed to get
the plugin to be exported and get recognised by gazebo
******
ament_export_libraries(simple_world)
install(DIRECTORY include/
        DESTINATION include)
******

USE THIS!! to run the simulation and see the custom plugin work 
----
gazebo --verbose src/testing_gazebo/worlds/test_world.world
----
