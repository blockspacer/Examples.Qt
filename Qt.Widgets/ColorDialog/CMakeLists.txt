cmake_minimum_required(VERSION 3.1)

# Project
project(ColorDialog)
find_package(Qt5Widgets CONFIG REQUIRED)

# Options
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Application
add_executable(ColorDialog WIN32 MACOSX_BUNDLE src/ColorDialog.cpp)
target_link_libraries(ColorDialog Qt5::Widgets)
