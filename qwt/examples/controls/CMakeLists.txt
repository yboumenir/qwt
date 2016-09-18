project(garbage)
#message(STATUS "source dir: ${CMAKE_SOURCE_DIR}")
#set(QWT_DIR ${CMAKE_SOURCE_DIR}/src/)

#include_directories(${QWT_DIR})
#message(STATUS "QWT_DIR: ${QWT_DIR}")

#file(GLOB QWT_SRC ${QWT_DIR}*.cpp
#                  ${QWT_DIR}*.h)

set(Y controls)
set(SRC
dialbox.cpp
dialbox.h
dialtab.cpp
dialtab.h
knobbox.cpp
knobbox.h
knobtab.cpp
knobtab.h
main.cpp
sliderbox.cpp
sliderbox.h
slidertab.cpp
slidertab.h
wheelbox.cpp
wheelbox.h
wheeltab.cpp
wheeltab.h)
add_executable(${Y} ${SRC})

#message(STATUS "bin dir: ${CMAKE_BINARY_DIR}")
#if(EXISTS "${CMAKE_BINARY_DIR}/src/libqwt.a")
#    message("lib qwt was found")
#else()
#    message(FATAL_ERROR "lib qwt was not found")
#endif()

target_link_libraries(${Y} qwt)
#qt5_use_modules( ${Y} Core Gui Widgets )



