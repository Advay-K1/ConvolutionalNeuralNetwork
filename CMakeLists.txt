cmake_minimum_required(VERSION 3.10)
project(ConvolutionalNeuralNetwork)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

find_package(Eigen3 3.3 REQUIRED NO_MODULE)

include_directories(${EIGEN3_INCLUDE_DIR})

add_executable(ConvolutionalNeuralNetwork main.cpp)

target_link_libraries(ConvolutionalNeuralNetwork Eigen3::Eigen)
