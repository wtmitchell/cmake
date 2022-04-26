cmake_minimum_required(VERSION 3.20)
project(C_Test_Project C)

# Add path for custom modules
set(CMAKE_MODULE_PATH
  ${CMAKE_MODULE_PATH}
  "${CMAKE_CURRENT_SOURCE_DIR}/../.."
  )

include(CompilerSetup)

add_executable(test_bin
  main.c
  )

enable_c_warnings_for(test_bin)
