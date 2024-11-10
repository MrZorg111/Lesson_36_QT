cmake_minimum_required(VERSION 3.21)

set(CMAKE_PREFIX_PATH "P:\\Qt\\5.15.2\\mingw81_64\\lib\\cmake")
find_package(Qt5 COMPONENTS Core Gui Widgets REQUIRED)
                 
                 


add_executable("Lesson_36_QT" main.cpp ${MY_INCLUDE_DIR}/function.h)
target_include_directories("Lesson_36_QT" PUBLIC ${MY_INCLUDE_DIR})
target_link_libraries("Lesson_36_QT" Qt5::Widgets Qt5::Core Qt5::Gui)