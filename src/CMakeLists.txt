add_compile_options(-std=c++14 -Wall -Wextra -Wshadow)

find_package(Threads REQUIRED)

add_executable(sample   main.cpp)
target_include_directories(sample PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})
target_link_libraries(sample PRIVATE Threads::Threads)