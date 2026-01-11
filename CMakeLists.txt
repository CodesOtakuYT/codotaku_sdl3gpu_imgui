cmake_minimum_required(VERSION 4.1)
project(codotaku_sdl3gpu_imgui)

set(CMAKE_CXX_STANDARD 23)

find_package(SDL3 CONFIG REQUIRED)
find_package(imgui CONFIG REQUIRED)

add_executable(codotaku_sdl3gpu_imgui main.cpp)
target_link_libraries(codotaku_sdl3gpu_imgui PRIVATE SDL3::SDL3 imgui::imgui)