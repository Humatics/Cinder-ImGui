cmake_minimum_required(VERSION 3.5)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

include_directories(include ../Cinder/include)

set(SOURCES src/CinderImGui.cpp)
set(HEADERS
        include/CinderImGui.h
        include/CinderImGuiExports.h
)

add_library(cinder_imgui src/CinderImGui.cpp)
target_link_libraries(cinder)
