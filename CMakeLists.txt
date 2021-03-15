cmake_minimum_required(VERSION 3.17)
project(CheckDeviceInfo CUDA)

set(CMAKE_CUDA_STANDARD 14)

add_executable(CheckDeviceInfo main.cu)

set_target_properties(
        CheckDeviceInfo
        PROPERTIES
        CUDA_SEPARABLE_COMPILATION ON)