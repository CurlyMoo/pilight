project(inc)

include(../CMakeConfig.txt)

if(WIN32)
	set(PILIGHT_ROOT "${CMAKE_INSTALL_PREFIX}")
else()
	set(PILIGHT_ROOT "${CMAKE_INSTALL_PREFIX}/lib")
endif()

configure_file(${PROJECT_SOURCE_DIR}/defines.h.in ${PROJECT_SOURCE_DIR}/defines.h)