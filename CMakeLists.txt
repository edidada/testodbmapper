cmake_minimum_required(VERSION 3.13)
project(testodbmapper)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -DDATABASE_MYSQL")

add_executable(testodbmapper driver.cxx)


target_link_libraries(testodbmapper libodb-mysql.so)

target_link_libraries(testodbmapper libodb.so)