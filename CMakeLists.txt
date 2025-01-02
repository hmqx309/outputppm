# 设置最低CMake版本
cmake_minimum_required(VERSION 3.10)

# 项目信息
project(ppmOutput VERSION 1.0 LANGUAGES CXX)

# 设置 C++ 标准
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# 添加源文件和头文件
add_executable(ppmOutput
    ppmOutput.cpp
    vec3.h
	color.h
)

# 包含头文件目录
target_include_directories(ppmOutput PUBLIC include)
