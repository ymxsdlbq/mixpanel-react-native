cmake_minimum_required(VERSION 3.4.1)
set(CMAKE_VERBOSE_MAKEFILE on)

file(GLOB rnoh_mixpanel_SRC CONFIGURE_DEPENDS *.cpp)
add_library(rnoh_mixpanel SHARED ${rnoh_mixpanel_SRC})
target_include_directories(rnoh_mixpanel PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
target_link_libraries(rnoh_mixpanel PUBLIC rnoh)

