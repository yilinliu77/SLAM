cmake_minimum_required (VERSION 3.10)
PROJECT(slam)

FILE(GLOB SOURCE_FILE *.cpp *.h ../include/*.h)

add_executable(${PROJECT_NAME} ${SOURCE_FILE})
target_include_directories(${PROJECT_NAME} PUBLIC ../include)
link_general(${PROJECT_NAME})
