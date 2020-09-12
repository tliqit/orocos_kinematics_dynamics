IF(ENABLE_EXAMPLES)
  INCLUDE_DIRECTORIES(${PROJ_SOURCE_DIR}/src ${PROJ_BINARY_DIR}/src)

  add_executable(geometry geometry.cpp )
  TARGET_LINK_LIBRARIES(geometry orocos-kdl)
  
  add_executable(trajectory_example trajectory_example.cpp )
  TARGET_LINK_LIBRARIES(trajectory_example orocos-kdl)

ENDIF(ENABLE_EXAMPLES)
