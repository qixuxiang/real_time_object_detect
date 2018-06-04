cmake_minimum_required(VERSION 3.2)
project(yolo)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")
set(SOURCE_FILES src/yolo_object_detection.cpp)
find_package(OpenCV 3.4 REQUIRED)
add_executable(yolo ${SOURCE_FILES})
target_link_libraries(${PROJECT_NAME} ${OpenCV_LIBS})
