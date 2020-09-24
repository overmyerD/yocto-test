cmake_minimum_required(VERSION 3.0.0)
project ("hello world")

add_executable(raptorconnect main.cpp)
#target_link_libraries(raptorconnect PRIVATE SDBusCpp::sdbus-c++)
set_property(TARGET raptorconnect PROPERTY CXX_STANDARD 17)
install(TARGETS raptorconnect DESTINATION bin)
