cmake_minimum_required(VERSION 3.1.0)

project(dbcc)

include_directories(
    include
)


file(GLOB SRC_FILES "src/*.c")

add_executable (${PROJECT_NAME}
    main.c
    ${SRC_FILES}
)