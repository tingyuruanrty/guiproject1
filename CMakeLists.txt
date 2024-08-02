cmake_minimum_required(VERSION 3.10)

project(MyQtProject)

set(CMAKE_CXX_STANDARD 11)

add_executable(Myqt main.cpp)

include_directories(${PROJECT_SOURCE_DIR})

find_package(Qt6 REQUIRED COMPONENTS Widgets)

target_link_libraries(Myqt Qt6::Widgets)