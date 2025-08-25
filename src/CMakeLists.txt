include_directories(.)
add_subdirectory(lib1)

add_executable(main main.cpp)
target_link_libraries(main lib1)