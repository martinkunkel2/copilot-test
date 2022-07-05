cmake_minimum_required(VERSION 3.14)
project(copilot-test VERSION 1.0.0)

include(GNUInstallDirs)

add_executable(copilot-test main.cpp)

install(TARGETS copilot-test EXPORT copilot-test
  LIBRARY DESTINATION lib
  ARCHIVE DESTINATION lib
  RUNTIME DESTINATION bin
  INCLUDES DESTINATION include
)
