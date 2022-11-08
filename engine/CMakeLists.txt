cmake_minimum_required(VERSION 3.22.0)
project(LunaLuxEngine CXX)

find_package(Vulkan)

set(engine_sources 
src/LunaLuxEngine.cpp

)

add_library(LunaLuxEngine ${engine_sources})
target_link_libraries(LunaLuxEngine libos ${Vulkan_LIBRARIES})
