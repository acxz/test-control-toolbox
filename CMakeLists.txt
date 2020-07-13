project(test_control_toolbox)
cmake_minimum_required(VERSION 2.8)

find_package(ct_optcon)

include_directories(${ct_optcon_INCLUDE_DIR})

add_executable(ex_NLOC NLOC.cpp)
target_link_libraries(ex_NLOC ct_optcon)
