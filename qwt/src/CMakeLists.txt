project(qwtlibs)
set(CMAKE_AUTOMOC ON)
set(QWT_DIR ${CMAKE_CURRENT_SOURCE_DIR})
link_directories(${CMAKE_CURRENT_BINARY_DIR})
message("QWT SRC DIR: " ${QWT_DIR})

file(GLOB QWT_SRC ${QWT_DIR}/*.cpp
                  ${QWT_DIR}/*.h)

include_directories(${QWT_DIR})
add_library(qwt ${QWT_SRC} )
qt5_use_modules(qwt Core Gui Widgets Network PrintSupport OpenGL OpenGLExtensions Svg)

target_link_libraries(qwt )

