# CMake 最低版本号要求
cmake_minimum_required(VERSION 2.8)

# 项目信息
project(Demo3)

# 查找当前目录下的所有文件并保存到DIR_SRCS变量
aux_source_directory(. DIR_SRCS)

# 指定生成目标
add_executable(Demo ${DIR_SRCS})
