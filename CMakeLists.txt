cmake_minimum_required(VERSION 3.6)
project(data_structure)

set(CMAKE_C_STANDARD 11)

set(SOURCE_FILES main.c testDemo.c)



#ADD_SUBDIRECTORY(HelloWorld)

include_directories(/usr/local/Cellar/cunit/2.1-3/include/)
link_directories(/usr/local/Cellar/cunit/2.1-3/lib/)
add_executable(data_structure ${SOURCE_FILES})
target_link_libraries(data_structure cunit)
#target_link_libraries(cunit libcunit)
