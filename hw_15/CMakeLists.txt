cmake_minimum_required(VERSION 3.5)

project(getstat LANGUAGES C)

set(This getstat)

add_executable(${This} main.c)

execute_process(COMMAND pg_config --pkgincludedir OUTPUT_VARIABLE PG_INCLUDE_DIR)

target_include_directories(${This} PUBLIC ${PG_INCLUDE_DIR} )

target_link_libraries(${This} pq)

target_compile_options(${This} PUBLIC -Wall -Wextra -Wpedantic -std=gnu11)
