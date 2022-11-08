cmake_minimum_required(VERSION 3.22.0)
project(TestGame CXX)

set(game_sources src/GameMain.cpp)

add_executable(TestGame ${game_sources})
target_link_libraries(TestGame LunaLuxEngine)