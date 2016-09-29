cmake_minimum_required(VERSION 3.3)

project(boost_iterator)

add_library(boost_iterator INTERFACE)

target_include_directories(boost_iterator BEFORE INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/include)

install(TARGETS boost_iterator DESTINATION lib)
install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/boost DESTINATION include)
