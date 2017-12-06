cmake_minimum_required(VERSION 3.8)
project(Cimg_test)

set(CMAKE_CXX_STANDARD 11)

set(CMAKE_CXX_FLAGS -O2)

find_package(OpenCV REQUIRED)

set(SOURCE_FILES main.cpp)
add_executable(Cimg_test ${SOURCE_FILES})

target_link_libraries(Cimg_test ${OpenCV_LIBS})