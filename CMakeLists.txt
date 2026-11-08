cmake_minimum_required(VERSION 3.29.0)
project(
    planning
    VERSION 0.0.1
    DESCRIPTION "a demo for cmake planning"
    HOMEPAGE_URL "https://github.com/qiuyue-1729/cmake_planning_demo"
    LANGUAGES CXX
)

set(CMAKE_CXX_STANDARD 17)

# 变量设置 动态库以及可执行文件的输出目录
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/bin)
set(Process_Dir ${CMAKE_SOURCE_DIR}/src/process)
set(PNC_Map_Dir ${CMAKE_SOURCE_DIR}/src/pnc_map)
# 添加子目录
add_subdirectory(src)