cmake_minimum_required(VERSION 3.3)
project(ImplApp)

include_directories("${PROJECT_SOURCE_DIR}")

#option (USE_WIDGET1 "Use Widget1" ON)
#option (USE_WIDGET2 "Use Widget2" OFF)

set(CMAKE_BUILD_TYPE Debug)

#add_executable(initialize_list initialize_list.cpp)
#set_property(TARGET initialize_list PROPERTY CXX_STANDARD 14)
#add_dependencies(initialize_list uniform_initialization)
add_definitions(-Wall)

add_executable(grid Grid.cpp Grid.h)
set_property(TARGET grid PROPERTY CXX_STANDARD 17)

add_executable(optional_example optional_example.cpp)
set_property(TARGET optional_example  PROPERTY CXX_STANDARD 17)

add_executable(deduction deduction.cpp)
set_property(TARGET deduction  PROPERTY CXX_STANDARD 17)


