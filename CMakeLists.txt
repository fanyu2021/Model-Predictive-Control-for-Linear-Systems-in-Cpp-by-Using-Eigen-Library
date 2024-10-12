cmake_minimum_required(VERSION 3.5)

project(linar_mpc)

find_package(Eigen3 REQUIRED)

add_executable(${PROJECT_NAME} driver_code.cpp ModelPredictiveController.cpp)
target_include_directories(${PROJECT_NAME} PUBLIC ${EIGEN3_INCLUDE_DIR})