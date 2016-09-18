project(garbage)

set(Y dials)
set(SRC ${Y}.cpp
attitude_indicator.cpp
attitude_indicator.h
cockpit_grid.cpp
cockpit_grid.h
compass_grid.cpp
compass_grid.h
dials.cpp
speedo_meter.cpp
speedo_meter.h)
add_executable(${Y} ${SRC})


target_link_libraries(${Y} qwt)


