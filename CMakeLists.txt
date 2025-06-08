cmake_minimum_required(VERSION 4.0)

project(HelloImgui)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

find_package(imgui CONFIG REQUIRED)

add_executable(HelloImgui main.cpp)

target_link_libraries(HelloImgui PRIVATE imgui::imgui)
