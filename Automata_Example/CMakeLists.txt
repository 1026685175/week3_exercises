cmake_minimum_required(VERSION 3.16) 
project(automata_exercise
  VERSION 0.0.1
  LANGUAGES CXX
)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin) # set output directory for executables 为可执行文档设置输出目录
set(CMAKE_CXX_STANDARD 17) # set C++ standard 为C++设置标准
set(CMAKE_CXX_STANDARD_REQUIRED ON) # set C++ standard required 为C++设置必须的标准

add_subdirectory(source) # add source directory 添加源文件目录

find_package(Catch2 3 REQUIRED PATHS /home/aq1026685175/CourseNote) # add 'PATHS /path/to/local/install' if required.   添加路径到本地安装
add_subdirectory(test) # add test directory 添加测试目录
