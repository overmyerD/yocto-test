cmake_minimum_required(VERSION 3.0.0)
project ("sdbus test")

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY bin)
set(CMAKE_CXX_FLAGS "-Wall -Wextra -Wpedantic -O3")

add_executable(main main.cpp)
#target_link_libraries(main PRIVATE SDBusCpp::sdbus-c++)
set_property(TARGET main PROPERTY CXX_STANDARD 17)
