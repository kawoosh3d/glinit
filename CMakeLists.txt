cmake_minimum_required(VERSION 3.1)
project(glinit)

set(CMAKE_CXX_STANDARD 14)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/shaders DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/)
add_executable(glinit main.cpp)
add_subdirectory(glad/)
target_link_libraries(glinit GL GLU glfw3 X11 Xxf86vm Xrandr pthread Xi Xinerama Xcursor glad dl)
