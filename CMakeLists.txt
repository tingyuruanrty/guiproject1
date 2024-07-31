cmake_minimum_required(VERSION 3.10)

project(MyQtProject)

set(CMAKE_PREFIX_PATH "C:/Qt/6.7.2/mingw_64")
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

# Find the Qt package
find_package(Qt6 COMPONENTS Widgets REQUIRED)

# Add the executable
add_executable(MyQtApp main.cpp)

# Link the Qt libraries
target_link_libraries(MyQtApp Qt6::Widgets)