project(garbage)

#set(QWT_DIR /home/yasser/source/qwt/qwt/src/)
#file(GLOB QWT_SRC ${QWT_DIR}/*.cpp
#                  ${QWT_DIR}/*.h)


set(Y simpleplot)
set(SRC ${Y}.cpp)
add_executable(${Y} ${SRC})
qt5_use_modules( ${Y} Core Gui Widgets )

target_link_libraries(${Y} qwt)



