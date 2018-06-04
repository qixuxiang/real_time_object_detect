cmake_minimum_required(VERSION 3.2)
project(yolov3)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")
set(SOURCE_FILES src/object_detection.cpp)
find_package(OpenCV 3.4 REQUIRED)
add_executable(yolov3 ${SOURCE_FILES})
target_link_libraries(${PROJECT_NAME} ${OpenCV_LIBS})
