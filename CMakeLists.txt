cmake_minimum_required(VERSION 3.5)

project(Qt-Ribbon LANGUAGES CXX)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(CMAKE_AUTOUIC ON)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
find_package(Qt5 COMPONENTS Widgets REQUIRED)

add_executable(Qt-Ribbon
  main.cpp
  mainwindow.cpp
  mainwindow.h
  mainwindow.ui
  ribbon.cpp
  ribbon.h
  ribbonbuttongroup.h
  ribbonbuttongroup.cpp
  ribbonbuttongroup.ui
  ribbontabcontent.h
  ribbontabcontent.cpp
  ribbontabcontent.ui
  resource.qrc
)
target_link_libraries(Qt-Ribbon Qt5::Widgets)
