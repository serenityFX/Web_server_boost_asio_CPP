cmake_minimum_required(VERSION 2.8)

project(final_x)

set(CMAKE_CXX_FLAGS "-std=c++11 -pthread")
set(SOURCE main.cpp connection.cpp mime_types.cpp reply.cpp request_handler.cpp request_parser.cpp server.cpp)
add_executable(final ${SOURCE})
target_link_libraries(final boost_system boost_thread)
