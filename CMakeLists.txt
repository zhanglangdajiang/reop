cmake_minimum_required(VERSION 3.16)
project(reop)

set(CMAKE_CXX_STANDARD 14)

#将<dir> 下的源文件保存到指定中 <variable>
aux_source_directory(./src DIR_SRCS)
aux_source_directory(./src/subdir DIR_SRCS)
#包含头文件
include_directories(include)


add_executable(tset ${DIR_SRCS})
