cmake_minimum_required(VERSION 3.10)

project(MyQtProject)

# Find the Qt package
find_package(Qt5 COMPONENTS Widgets REQUIRED)

# Add the executable
add_executable(MyQtApp main.cpp)

# Link the Qt libraries
target_link_libraries(MyQtApp Qt5::Widgets)