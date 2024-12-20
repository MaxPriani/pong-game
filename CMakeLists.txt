cmake_minimum_required(VERSION 3.10)
project(pong)

set(CMAKE_C_STANDARD 99)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/build)

set(SRC_DIR ${CMAKE_CURRENT_SOURCE_DIR}/src)
set(INCLUDE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/include)

 set(SRC_FILES
    ${SRC_DIR}/init.c
    ${SRC_DIR}/main.c
    ${SRC_DIR}/ball.c
    ${SRC_DIR}/paddle.c
    ${SRC_DIR}/game_init.c
    ${SRC_DIR}/game.c
 )

include_directories(${SRC_DIR})
include_directories(${INCLUDE_DIR})

find_package(SDL2 REQUIRED)
find_package(SDL2_ttf REQUIRED)

include_directories(${SDL2_INCLUDE_DIRS} ${SDL2_TTF_INCLUDE_DIRS})

add_executable(pong ${SRC_FILES})

target_link_libraries(pong ${SDL2_LIBRARIES} ${SDL2_TTF_LIBRARIES})
