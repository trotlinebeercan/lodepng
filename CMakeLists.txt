cmake_minimum_required (VERSION 3.1)

project (lodepng)

set (CMAKE_CXX_STANDARD 11)
set (CMAKE_CXX_STANDARD_REQUIRED on)

set (CMAKE_BUILD_TYPE Release)

add_library (lodepng STATIC lodepng.cpp)

install (TARGETS lodepng
    RUNTIME DESTINATION bin
    LIBRARY DESTINATION lib
)
install (FILES lodepng.h DESTINATION include)
