cmake_minimum_required(VERSION 3.16)
project(test)

set(CMAKE_CXX_STANDARD 20)


find_package(Qt5 COMPONENTS Core Widgets Qml Quick QuickControls2 REQUIRED)

add_executable(test main.cpp)
target_link_libraries(test Qt5::Core Qt5::Widgets Qt5::Qml Qt5::Quick Qt5::QuickControls2)
