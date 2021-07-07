cmake_minimum_required(VERSION 3.10)
project(maxwell2021)


# 设置库文件输出目录
set(LIBRARY_OUTPUT_PATH ${CMAKE_BINARY_DIR}/${CMAKE_BUILD_TYPE}/lib)
set(RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/${CMAKE_BUILD_TYPE}/lib)

# 设置执行文件输出目录
set(EXECUTABLE_OUTPUT_PATH ${CMAKE_BINARY_DIR}/${CMAKE_BUILD_TYPE}/bin)

# 设置版本号
set(VERSION_SHORT 1)

# 设置qt目录
set(CMAKE_PREFIX_PATH "C:\\Qt\\5.15.2\\msvc2019_64")

# 设置Qt-Advanced-Docking-System静态编译
option(BUILD_STATIC "Build the static library" ON)

# 添加子目录
add_subdirectory(src)
add_subdirectory(Qt-Advanced-Docking-System-3.7.1)
