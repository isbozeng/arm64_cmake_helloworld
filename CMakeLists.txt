cmake_minimum_required(VERSION 3.0)

project(helloworld)
# 设置交叉编译工具链
set(CMAKE_SYSTEM_NAME Linux)
set(CMAKE_SYSTEM_PROCESSOR aarch64)

# 设置交叉编译工具的前缀，根据您的工具链配置
set(CMAKE_C_COMPILER aarch64-linux-gnu-gcc)
set(CMAKE_CXX_COMPILER aarch64-linux-gnu-g++)


# 添加可执行文件，指定源文件
add_executable(${PROJECT_NAME} hello.cpp)

