IF(ENABLE_EXAMPLES)
  find_package(Boost REQUIRED)
  include_directories(${Boost_INCLUDE_DIRS})
  
  INCLUDE_DIRECTORIES(${PROJ_SOURCE_DIR}/src ${PROJ_SOURCE_DIR}/models ${PROJ_BINARY_DIR}/src)

  add_executable(geometry geometry.cpp )
  TARGET_LINK_LIBRARIES(geometry orocos-kdl)
  
  add_executable(trajectory_example trajectory_example.cpp )
  TARGET_LINK_LIBRARIES(trajectory_example orocos-kdl)

ENDIF(ENABLE_EXAMPLES)
