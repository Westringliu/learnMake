# CMake 最低版本号要求
cmake_minimum_required(VERSION 2.8)

# 项目信息
project(Demo4)

# 添加头文件目录
include_directories ("${PROJECT_SOURCE_DIR}/math")

# 查找当前目录下的所有文件并保存到DIR_SRCS变量
aux_source_directory(. DIR_SRCS)

# 添加 math 子目录
add_subdirectory(math)

# 指定生成目标
add_executable(Demo main.cc)

# 添加连接库
target_link_libraries(Demo MathFunctions)
