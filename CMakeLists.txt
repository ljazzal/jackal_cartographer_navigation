cmake_minimum_required(VERSION 2.8.3)
project(jackal_cartographer_navigation)

find_package(catkin REQUIRED COMPONENTS roslaunch)

catkin_package()

roslaunch_add_file_check(launch/cartographer_demo.launch)

install(DIRECTORY launch config
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
