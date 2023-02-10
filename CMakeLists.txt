cmake_minimum_required(VERSION 3.15)

project(TestPlotGraph C CXX)

add_executable(TestPlotGraph)

add_subdirectory(Src)
add_subdirectory(Dependencies/sciplot)

target_link_libraries(TestPlotGraph PRIVATE
    sciplot
    CommonAplication
)


