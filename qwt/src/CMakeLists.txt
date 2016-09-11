project(qwtlibs)

set(QWT_DIR ${CMAKE_CURRENT_SOURCE_DIR})

message("QWT SRC DIR: " ${QWT_DIR})

file(GLOB QWT_SRC ${QWT_DIR}/*.cpp
                  ${QWT_DIR}/*.h)

#include_directories(${QWT_DIR})
add_library(qwt ${QWT_SRC} )

target_link_libraries(qwt )
