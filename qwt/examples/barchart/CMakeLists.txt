project(garbage)
set(Y barchart)
set(SRC
    ${Y}.cpp
    ${Y}.h
    main.cpp)
add_executable(${Y} ${SRC})
target_link_libraries(${Y} qwt)


