### GTK ###
find_package(GTK2)
if(GTK2_FOUND)
    include_directories(${GTK2_INCLUDE_DIRS})
else()
    message(STATUS "Could not find GTK2; will not build browser plugin on Linux")
endif()

include_directories(SYSTEM ${GTK2_INCLUDE_DIRS} ${CMAKE_SOURCE_DIR}/src/firebreath)
