set(FB_PROJECTS_DIR "${CMAKE_SOURCE_DIR}/src")
add_definitions(-DQT_NO_KEYWORDS)

if(MSVC)
    set_msvc_warning_level(0)
endif()

if(CMAKE_COMPILER_IS_CLANGXX OR CMAKE_COMPILER_IS_GNUCXX)
    set_gcc_warning_level("none")
endif()

if(CMAKE_COMPILER_IS_CLANGXX)
    set_clang_warning_level("none")
endif()

add_subdirectory(firebreath)
