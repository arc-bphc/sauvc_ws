add_executable(sim_remote_control   ${COMMON_SRC_FILES}
									${COMMON_VEC6_SIM_FILES}
									sim_remote_control.cpp)

target_link_libraries(sim_remote_control ${catkin_LIBRARIES})
find_package(catkin  REQUIRED COMPONENTS
  roscpp
)

include_directories(include ${catkin_INCLUDE_DIRS} )